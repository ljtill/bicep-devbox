# Dev Box

## Introduction

This repository contains the modules and tools to quickly scaffold a new [Microsoft Dev Box](https://azure.microsoft.com/services/dev-box/) environment.

### Getting Started

1. Configure Azure Active Directory
    1. Create a new application
    2. Setup the federated credentials
2. Configure GitHub Actions
    1. Add the following repository secrets
        - ARM_TENANT_ID
        - ARM_SUBSCRIPTION_ID
        - ARM_CLIENT_ID
3. Configure Azure Deployment
    1. Update `src/azureconfig.json` file with required values

### Resources

The following resources will be provisioned as part of the deployment.

- Virtual Network
- Network Security Group
- Managed Identity (User)
- Network Connection
- DevCenter
- DevCenter Definitions
- DevCenter Project
- DevCenter Pools

## Useful Links

- [Microsoft Dev Box](https://docs.microsoft.com/azure/dev-box)
- [Azure Bicep](https://docs.microsoft.com/azure/azure-resource-manager/bicep)
- [OpenID Connect](https://docs.github.com/actions/deployment/security-hardening-your-deployments/configuring-openid-connect-in-azure)