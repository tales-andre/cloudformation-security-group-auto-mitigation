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