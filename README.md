# rms-k8s-iac
Contains the Kubernetes cluster related Infrastructure as code (IaC) of the [RMS project](https://github.com/Grupo-G03-4SOAT-FIAP/rms-bff).

[![Terraform Apply](https://github.com/Grupo-G03-4SOAT-FIAP/rms-k8s-iac/actions/workflows/terraform-apply.yml/badge.svg)](https://github.com/Grupo-G03-4SOAT-FIAP/rms-k8s-iac/actions/workflows/terraform-apply.yml)
[![Terraform Plan](https://github.com/Grupo-G03-4SOAT-FIAP/rms-k8s-iac/actions/workflows/terraform-plan.yml/badge.svg)](https://github.com/Grupo-G03-4SOAT-FIAP/rms-k8s-iac/actions/workflows/terraform-plan.yml)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=Grupo-G03-4SOAT-FIAP_rms-k8s-iac&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=Grupo-G03-4SOAT-FIAP_rms-k8s-iac)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=Grupo-G03-4SOAT-FIAP_rms-k8s-iac&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=Grupo-G03-4SOAT-FIAP_rms-k8s-iac)

![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=for-the-badge&logo=terraform&logoColor=white)

> [!IMPORTANT]  
> O código nesse repositório foi movido e unificado em https://github.com/Grupo-G03-4SOAT-FIAP/rms-iac

[Ver no Terraform Cloud](https://app.terraform.io/app/Grupo-G03-4SOAT-FIAP/workspaces/rms-k8s)↗️

## Pré-requisitos

Você deve ter instalado o [Terraform CLI](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli), a [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html), o [kubectl](https://kubernetes.io/docs/tasks/tools/) e possuir uma conta na AWS.

Antes de começar, você precisa definir duas variáveis de ambiente em seu computador: `AWS_ACCESS_KEY_ID` e `AWS_SECRET_ACCESS_KEY`. Elas devem conter o **ID da chave de acesso** do seu usuário do IAM na AWS e sua respectiva **Chave de acesso secreta**. Você pode obtê-los na seção "[Minhas credenciais de segurança](https://us-east-1.console.aws.amazon.com/iam/home#/security_credentials)" no console da AWS conforme instruções na página [Managing access keys for IAM users](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html#Using_CreateAccessKey).

```bash
export AWS_ACCESS_KEY_ID=???
```

```bash
export AWS_SECRET_ACCESS_KEY=???
```

> Substitua os sinais de interrogação `???` acima pelas suas credenciais do IAM da AWS.

## Como aplicar o plano de execução do Terraform manualmente

1. Clone este repositório;
2. Navegue até a pasta raiz do projeto;
3. Use o comando `terraform apply` para aplicar o plano de execução;

> Para excluir a infraestrutura provisionada pelo Terraform, use o comando `terraform destroy`

## Projetos relacionados

BFF do Restaurant Management System (RMS)\
https://github.com/Grupo-G03-4SOAT-FIAP/rms-bff

## Requisitos

*Terraform 1.7.3*\
*aws-cli/2.15.10*

[![SonarCloud](https://sonarcloud.io/images/project_badges/sonarcloud-white.svg)](https://sonarcloud.io/summary/new_code?id=Grupo-G03-4SOAT-FIAP_rms-k8s-iac)
