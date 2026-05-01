# ARQUITETURA LAMBDA + S3
Arquitetura simples orientada a eventos utilizando serviços da AWS para receber solicitações de orçamento com upload de imagens.

## Objetivo
Permitir que usuários enviem formulários de orçamento com imagens de forma escalável, segura e com baixo custo operacional.

# Fluxo Resumido
Usuário → Frontend → Lambda (gera upload URL) → S3 (upload imagem) → Lambda (validação) → DynamoDB → SNS

# Arquitetura EC2 + RDS
Arquitetura tradicional baseada em instâncias persistentes para um sistema ERP interno com múltiplos usuários simultâneos, processamento contínuo e armazenamento centralizado.

## Objetivo
Disponibilizar um sistema ERP confiável e persistente para uso contínuo dos funcionários da empresa.

# Fluxo Resumido
Usuário → Load Balancer → EC2 (ERP Backend) → RDS
