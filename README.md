# Global Azure Bootcamp 2017
## Build and Release the Azure way

En el siguiente lab vamos realizar el build de una web api y deployearlo en azure en los entornos de Dev, QA y Prod.

Se utiliza azure como ejemplo pero el deployment se puede realizar en cualquier plataforma. Aws, Google, Onpremises, ios y Android.

## Requisitos
Una cuenta de [link vsts]. El servicio es gratuito para 5 developers e ilimitados Stakeholders.
Una cuenta de Azure para deploy de Azure Web App

## Paso 1
Clonar el repositorio
1. Ingrear la url de Github https://github.com/barchito/gab-2017
2. Aceptar los cambios.
3. Esperar mientras hace el clone

## Paso 2
Revisar que

![Paso 1](docs/1-create-build.png)




## Paso 3

# Configuraciones especiales de las tareas

Build solution

/p:DeployOnBuild=true /p:WebPublishMethod=Package /p:PackageAsSingleFile=true /p:SkipInvalidConfigurations=true /p:PackageLocation=$(build.stagingDirectory)

Copy Tools
$(build.sourcesDirectory)\ResourceGroup\
*.json

[link vsts](https://www.visualstudio.com/es/team-services/)