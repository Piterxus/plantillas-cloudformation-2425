# ☁️ Prácticas con AWS CloudFormation

Este repositorio contiene una colección de prácticas realizadas con **AWS CloudFormation**, enfocadas en la automatización y despliegue de infraestructura en **Amazon Web Services (AWS)** mediante plantillas declarativas escritas en YAML.

Cada carpeta incluye una plantilla o conjunto de archivos que representa una práctica concreta de clase.

---

## 📁 Estructura del repositorio

Este repositorio contiene una colección de prácticas realizadas con **AWS CloudFormation**, enfocadas en la automatización y despliegue de infraestructura en **Amazon Web Services (AWS)** mediante plantillas declarativas escritas en YAML.

Cada carpeta incluye una plantilla o conjunto de archivos que representa una práctica concreta de clase.

```txt
cloudformation/
├── ejercicios/ # Plantillas variadas de recursos básicos
├── ejercicios_sistemas/ # Configuración de sistemas más complejos
├── practica_4_2/ # Práctica específica 4.2 con recursos definidos
├── practica_4_3/ # Práctica específica 4.3 centrada en configuración avanzada
├── practica_RDS/ # Despliegue de base de datos RDS con parámetros
├── practica_redes/ # Configuración de red: VPC, subredes, IGW, etc.
├── .gitignore # Exclusiones para Git
└── README.md # Este documento
```

---

## 🛠 Requisitos

- Cuenta activa de AWS con permisos para usar CloudFormation
- AWS CLI configurado con `aws configure`
- [CloudFormation Linter (cfn-lint)](https://github.com/aws-cloudformation/cfn-lint) para validar plantillas (opcional)
- Editor recomendado: Visual Studio Code con extensión de YAML y AWS

---

## 🚀 Cómo desplegar una plantilla

1. **Clona este repositorio:**

   ```bash
   git clone https://github.com/tu-usuario/cloudformation-practicas.git

   cd cloudformation # Navega a la carpeta del repositorio

   cd practica_RDS # Navega a la carpeta de la práctica

   aws cloudformation deploy \
     --template-file template.yaml \
     --stack-name nombre-de-tu-stack \
     --capabilities CAPABILITY_NAMED_IAM # Despliega la plantilla con AWS CLI (Reemplaza con el nombre de tu stack)

   aws cloudformation delete-stack --stack-name nombre-de-tu-stack # Elimina el stack creado (opcional)

## 📚 Descripción de prácticas

Carpeta	Descripción
ejercicios	Plantillas básicas con recursos como EC2, S3, IAM
ejercicios_sistemas	Ejercicios orientados a configuraciones de sistemas
practica_4_2	Práctica específica centrada en configuración de red o servicios definidos
practica_4_3	Ejercicio avanzado con múltiples recursos conectados entre sí
practica_RDS	Despliegue de una base de datos Amazon RDS con parámetros personalizables
practica_redes	Plantilla para crear VPC, subredes, gateway, tablas de ruta, etc.

## 🔒 Buenas prácticas

No incluyas claves ni secretos en las plantillas.

Usa Parameters para mayor flexibilidad en las configuraciones.

Utiliza Outputs para obtener valores útiles como IPs o nombres de recursos.

Valida tus plantillas con cfn-lint antes de desplegar.

Elimina stacks innecesarios para evitar costes inesperados.

## 📜 Licencia

Este proyecto está licenciado bajo la [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).




