# aws-comprehend-analyze-text

Este repositorio contiene un ejemplo de cómo utilizar:
1. [AWS Comprehend](https://aws.amazon.com/comprehend/) para analizar texto en una función 
2. [AWS Lambda](https://aws.amazon.com/lambda/) y exponerla a través de API Gateway
3. [AWS API Gateway](https://aws.amazon.com/api-gateway/) en una arquitectura [serverless](https://aws.amazon.com/serverless/).

## Funcionalidades
- Análisis de sentimiento (positivo, negativo, neutro) en texto en español
- Análisis de entidades (personas, lugares, organizaciones, etc) en texto en español

## Pre-requisitos
- Una cuenta de AWS activa
- AWS CLI configurado en su computadora
- Un ambiente de desarrollo con Node.js y npm instalado

## Instrucciones
1. Clona este repositorio a tu computadora
2. Ejecuta `npm install` en la raíz del proyecto para instalar las dependencias
3. Ejecuta `serverless deploy` para desplegar el código a AWS

Una vez completado estos pasos, se te proporcionará una URL en la salida del comando `serverless deploy` que puedes usar para hacer llamadas a la función desplegada.

Ejemplo de uso: 
````
curl -X POST https://<api-id>.execute-api.<region>.amazonaws.com/dev/analyze-text -d '{"text": "Este es un ejemplo de texto a analizar"}'
````


## Cómo contribuir
Siéntete libre de abrir una issue o un pull request si deseas contribuir al proyecto. 🚀

## Licencia
Este proyecto está licenciado bajo la licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.


