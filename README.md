# Deploy to Azure

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fdeathmarine%2Fcloud-actual-budget%2Fmain%2Farm-templates%2Fazuredeploy.json)


This template deploys:
- An Azure App Service (Linux, Free tier) running the container image `docker.io/actualbudget/actual-server:latest`
- An Azure Storage Account with a file share named `actual-data` (transaction optimized)
- Mounts the file share to the App Service at `/data`
