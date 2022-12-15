# Despliegue de una aplicación web multicapa altamente disponible y segura mediante AWS Elastic Beanstalk con AWS Academy Learner Labs

## Objetivo:
AWS Elastic Beanstalk es un servicio que permite a los desarrolladores desplegar y administrar rápidamente aplicaciones en la nube de AWS sin necesidad de gestionar la infraestructura en la que se ejecutan las aplicaciones, reduciendo con ello la complejidad y sobrecarga administrativa que conlleva el aprovisionamiento, balanceo de carga, escalado y monitorización de la aplicación.

AWS Elastic Beanstalk permite desplegar aplicaciones desarrolladas en Java, PHP, .NET, Ruby, Python, Go y Node.js bajo instancias de Amazon EC2.

Es posible interactuar con AWS Elastic Beanstalk de la misma forma que con el resto de los servicios; es decir, mediante la Consola de Administración de AWS, mediante la AWS CLI y programáticamente desde los SDKs. Adicionalmente, AWS pone a nuestra disposición una interfaz de línea de comandos de más alto nivel especialmente diseñada para AWS Elastic Beanstalk desde la que podemos desplegar con facilidad y rapidez las aplicaciones.

El objetivo de esta práctica es, precisamente, dar a conocer las posibilidades de esta herramienta desplegando una sencilla aplicación web multicapa sin estado desarrollada en PHP utilizando AWS Elastic Beanstalk, junto con otros servicios para diseñar una infraestructura altamente disponible, escalable y segura en el entorno de AWS Academy Learner Labs.

## Solución a implementar:
La solución que se implementará utilizará los siguientes servicios:
* **AWS Elastic Beanstalk**, para el aprovisionamiento y escalado de la infraestructura computacional, balanceo de carga, despliegue de la aplicación web en PHP. Este servicio aprovisionará instancias de Amazon EC2 y un balanceador de carga.
* **Amazon RDS**, para el aprovisionamiento y administración de una base de datos relacional con un motor MariaDB en alta disponibilidad.
* **Amazon VPC**, para la administración y creación de una infraestructura de red altamente disponible y segura.
* **AWS CloudFormation**, para el despliegue automatizado de la infraestructura de red anterior. Además, AWS Elastic Beanstalk también utiliza AWS CloudFormation tras las bambalinas.
* **Amazon CloudWatch Logs y Metrics**, para obtener visibilidad sobre el rendimiento y desempeño tanto de la infraestructura como de la aplicación desplegada.
* **AWS Systems Manager Parameter Store**, para proteger las credenciales de acceso a la base de datos de la aplicación.
* **Amazon S3**, para alojar las diferentes versiones de las aplicaciones que se despliegan en AWS Elastic Beanstalk.
* **Amazon CloudFront**, para brindar seguridad en el borde y rendimiento a nivel global a nuestra aplicación.

La arquitectura propuesta queda reflejada en la siguiente figura:
 
![Arquitectura](/images/arch.png)
