# Blazor WASM Deployment
This is a sample application that uses Blazor WASM app with no host to publish as a static site to Azure Storage.  A complimentary blog post explaining this can be found here [Deploy a Blazor WASM site to Azure Storage using GitHub Actions](https://timheuer.com/blog/deploy-blazor-app-to-azure-using-github-actions).

## How this works
This sample takes a Blazor Web Assembly project and uses GitHub Actions to deploy it in a few ways:

- [Azure Storage](.github/workflows/azure-storage-deploy.yml)
- [Azure App Service (Linux)](.github/workflows/azure-app-svc-linux-deploy.yml)
- [Azure App Service (Linux) using Containers](.github/workflows/azure-app-svc-linux-container.yml)

You can see each of the steps in the .github/workflows files linked above.

## Requirements
The following is required (and/or pre-requisite) to get this working similarly:

- An Azure Account - get one [Free](https://azure.com/free)
- An Azure Service Principal and stored in repo Secrets as ```AZURE_CREDENTIALS```
- An Azure Storage resource [configured to use Static Sites](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blob-static-website)

## Contact
This was done by [Tim Heuer](https://twitter.com/timheuer) as a sample and to play around with different deployment options.  If you have ideas, reach out!