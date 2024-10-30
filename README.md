# CloudFormation Security Group Auto Mitigation

This project provides an AWS CloudFormation template that monitors and automatically mitigates unwanted changes to Security Groups. It ensures that only specific ports are publicly accessible (0.0.0.0/0) and revokes rules that do not meet this criterion.

## Features

- **Real-Time Monitoring**: Utilizes AWS Lambda and Amazon EventBridge to monitor changes in Security Groups.
- **Auto-Mitigation**: Automatically revokes ingress rules that are not on the allowed ports or that expose other ports to the public IP.
- **Customizable Configuration**: Easy to adjust to add or remove allowed ports.

## Allowed Ports

- **80** (HTTP)
- **443** (HTTPS)
- **53** (DNS)
- **123** (NTP)
- **993** (IMAPS)
- **995** (POP3S)
- **1194** (OpenVPN)
- **1935** (RTMP)

## Prerequisites

- AWS account with permissions to create IAM, Lambda, and CloudFormation resources.
- AWS CLI configured (optional but recommended).

## How to Use

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/repository-name.git
   cd repository-name


# CloudFormation Security Group Auto Mitigation

Este projeto fornece um template AWS CloudFormation que monitora e automaticamente mitiga alterações indesejadas em Security Groups. Ele garante que apenas portas específicas estejam acessíveis publicamente (0.0.0.0/0) e revoga regras que não atendam a esse critério.

## Funcionalidades

- **Monitoramento em Tempo Real**: Utiliza AWS Lambda e Amazon EventBridge para monitorar alterações nos Security Groups.
- **Auto-Mitigação**: Revoga automaticamente regras de ingresso que não estão nas portas permitidas ou que expõem outras portas para o IP público.
- **Configuração Personalizável**: Fácil de ajustar para adicionar ou remover portas permitidas.

## Portas Permitidas

- **80** (HTTP)
- **443** (HTTPS)
- **53** (DNS)
- **123** (NTP)
- **993** (IMAPS)
- **995** (POP3S)
- **1194** (OpenVPN)
- **1935** (RTMP)

## Pré-requisitos

- Conta AWS com permissões para criar recursos IAM, Lambda, e CloudFormation.
- AWS CLI configurada (opcional, mas recomendado).

## Como Usar

1. **Clone o Repositório**

   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio

