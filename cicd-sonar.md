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

## Sonar 
    - Agregar el proyecto ...
### Instalar sonnar-scanner
  * cd /opt/
  *  sudo curl -o sonar-scarnner.zip https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-6.2.1.4610-linux-x64.zip?_gl=1*1euibzl*_gcl_au*MjA0NzM0NTQxMS4xNzMyODI3MDg3*_ga*NjkxOTU2OTguMTcyMTY4NDQxMA..*_ga_9JZ0GZ5TC6*MTczODA3NjgzNS4yMS4xLjE3MzgwNzc4MjkuNTkuMC4w
  * sudo apt-get install zip
  * sudo unzip sonar-scarnner.zip
  * sudo nano /etc/profile
  * source /etc/profile

### Instalar sonnar-runner