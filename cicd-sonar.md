## Pasos previos
### Hacer los pull con SSH

ssh-keygen -t rsa -b 4096 -C "otidg15@igp.gob.pe"

Copiar
 cat ~/.ssh/id_rsa.pub


Ve a tu cuenta de GitLab.
* Haz clic en tu foto de perfil (arriba a la derecha) y selecciona "Preferences" o "Configuración".
* En el menú de la izquierda, selecciona "SSH Keys".
* Copia el contenido de tu clave pública (id_ed25519.pub) y pégalo en el campo Key.


- En la maquina con VPN tener registrado en hosts code y sonar

## Instalar node
* curl -sL https://deb.nodesource.com/setup_18.x | sudo bash -
* sudo apt install -y nodejs
* node -v
* Revisar uso de node.js para javascript: https://docs.sonarsource.com/sonarqube-server/9.9/analyzing-source-code/scanner-environment/



## Sonar 
    - Agregar el proyecto ...

### Instalar sonnar-scanner
  * cd /opt/
  *  sudo curl -o sonar-scarnner.zip https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-6.2.1.4610-linux-x64.zip?_gl=1*1euibzl*_gcl_au*MjA0NzM0NTQxMS4xNzMyODI3MDg3*_ga*NjkxOTU2OTguMTcyMTY4NDQxMA..*_ga_9JZ0GZ5TC6*MTczODA3NjgzNS4yMS4xLjE3MzgwNzc4MjkuNTkuMC4w
  * sudo apt-get install zip
  * sudo unzip sonar-scarnner.zip
  * sudo nano /etc/profile
        export SONAR_SCANNER_HOME="/opt/sonar-scanner-6.2.1.4610-linux-x64"
        export PATH="$SONAR_SCANNER_HOME/bin:$PATH"
  * source /etc/profile
 
## Deploy

### Instalar sonnar-runner Debian
 - https://docs.gitlab.com/runner/install/linux-repository.html?tab=Debian%2FUbuntu%2FMint
 - 'curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash'
 - sudo apt install gitlab-runner
 - apt-cache madison gitlab-runner
 - sudo apt install gitlab-runner
### Registrar runner

* Importante registrar el runner con sudo, para que al desplegar el usuario de runnergit pueda tener acceso
* Importante crear una llave ssh para el usuario runner
* Todos los usuarios podrán ejecutar comandos en sudo chmod o+x /home/eis
