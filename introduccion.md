# SonarQube


>  ### ***Escribir código funcional no es suficiente.***
> - Confiable
> - Seguro
> - Mantenible


[Fuente de la documentación](https://docs.sonarsource.com/sonarqube-server/latest/ "Página oficial de SonarQube")

**SonarQube** es un sistema de análisis de código que nos ayuda a identificar problemas en más de 30 lenguajes de programación y frameworks.

Nos permite no solo **detectar errores**, sino también **mejorar continuamente** la calidad de nuestro código.


## El enfoque clean code
El código limpio es el estándar que garantiza que el software sea seguro, confiable y mantenible. Es esencial para mantener una base de código saludable.
La solución Sonar está diseñada para ayudarte a alcanzar un estado de Código Limpio

![Atributos](cleancodeatt.webp)

### Beneficios del código limpio: las cualidades del software
![Beneficios](cleancodebenet.webp)

### Severidad a nivel de calidad

| **Severidad**  | **Definición**                                                                                       |
|----------------|-----------------------------------------------------------------------------------------------------|
| **Bloqueador**  | Error con una alta probabilidad de afectar el comportamiento de la aplicación en producción.        |
| **Alto**        | Error con una baja probabilidad de afectar el comportamiento de la aplicación en producción o un problema que representa una falla de seguridad. |
| **Medio**       | Un defecto de calidad que puede afectar en gran medida a la productividad del desarrollador.         |
| **Bajo**        | Un defecto de calidad que puede afectar ligeramente a la productividad del desarrollador.           |
| **Información** | Ni un error ni un defecto de calidad, solo un hallazgo.                                             |

### Análisis de código basado en código limpio


* Cada atributo de código limpio se evalúa, para un lenguaje dado, en función de una serie de reglas
    <details>
    <summary>Reglas: (Haz clic para expandir)</summary>
    
   Cada regla
    
    - Está asociado con el atributo de código limpio que evalúa.
    - Está asociada con la(s) cualidad(es) del software a las que este atributo de Clean Code contribuye.
    Cada cualidad del software asociada (seguridad, confiabilidad o mantenibilidad) recibe un nivel de severidad (crítico, alto, medio, bajo o informativo). Esta severidad determina cuánto se ve afectada esa cualidad del software cuando se incumple la regla.

    </details>
* Si se incumple una regla, se genera un problema(issue).
* Este problema afecta una o más cualidades del software con diferentes * niveles de severidad.

## Clean as You Code

Práctica de desarrollo de software basada en el principio de que el código nuevo (código que ha agregado o modificado recientemente) debe cumplir con los estándares de calidad. La solución Sonar implementa Clean as You Code advirtiéndole cada vez que se detectan problemas en su nuevo código.

![cleanasucode](cleanasucode.webp)
*Diagrama de Clean as You Code.*
<details>
    <summary>Sobre los estándares de calidad: (Haz clic para expandir)
    </summary>    
    
    En la solución Sonar, cada uno de sus proyectos tiene un estándar de calidad establecido, compuesto por un perfil de calidad y una puerta de calidad:
    
    - Un perfil de calidad determina el conjunto de reglas que se aplican durante el análisis.
    - Una puerta de calidad consiste en un conjunto de condiciones con las que se mide el código durante el análisis. Dependiendo del resultado, el código pasará o no la puerta de calidad, lo que dará a los desarrolladores indicaciones sobre si deben solucionar problemas o fusionar el código.
    (Sonar way)   

</details>





