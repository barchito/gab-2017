Configuraciones especiales de las tareas

Build solution
/p:DeployOnBuild=true /p:WebPublishMethod=Package /p:PackageAsSingleFile=true /p:SkipInvalidConfigurations=true /p:PackageLocation=$(build.stagingDirectory)

Copy Tools
$(build.sourcesDirectory)\ResourceGroup\
*.json
