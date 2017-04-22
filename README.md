# Global Azure Bootcamp 2017.
## Build and Release the Azure way

En el siguiente lab vamos realizar el build de una web api y deployearlo en azure en los entornos de Dev, QA y Prod.

Se utiliza azure como ejemplo pero el deployment se puede realizar en cualquier plataforma. Aws, Google, Onpremises, ios y Android.

# Configuraciones especiales de las tareas

Build solution

/p:DeployOnBuild=true /p:WebPublishMethod=Package /p:PackageAsSingleFile=true /p:SkipInvalidConfigurations=true /p:PackageLocation=$(build.stagingDirectory)

Copy Tools
$(build.sourcesDirectory)\ResourceGroup\
*.json
