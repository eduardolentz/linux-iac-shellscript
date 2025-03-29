# linux-iac-shellscript

Este repositório contém dois scripts em Bash que simulam a criação de uma infraestrutura básica em ambiente Linux, seguindo os princípios de **Infraestrutura como Código (IaC)**.

Este desafio faz parte do bootcamp da **Digital Innovation One (DIO)**.

## 🧱 Objetivo

Automatizar o provisionamento de:

- Diretórios
- Grupos de usuários
- Usuários do sistema
- Permissões de acesso aos diretórios

## 📁 Estrutura

- `iac1.sh`: Cria diretórios, grupos de usuários, os usuários de cada grupo e define as permissões corretas.
- `criar_user.sh`: Cria usuários convidados com senha padrão e força a troca no primeiro login.

## 📂 Diretórios Criados

- `/publico`
- `/adm`
- `/ven`
- `/sec`

## 👥 Grupos de Usuários

- `GRP_ADM`
- `GRP_VEN`
- `GRP_SEC`

## 👤 Usuários

| Grupo      | Usuários                        |
|------------|---------------------------------|
| GRP_ADM    | carlos, maria, joao             |
| GRP_VEN    | debora, sebastiana, roberto     |
| GRP_SEC    | josefina, amanda, rogerio       |
| Convidados | guest10, guest11, guest12, guest13 |

## 🔐 Permissões

- O diretório `/publico` tem permissão total para todos (`chmod 777`)
- Cada diretório de grupo tem permissão `770` e pertence ao grupo correspondente

## ▶️ Como usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/eduardolentz/linux-iac-shellscript.git
   cd linux-iac-shellscript
   ```

2. Dê permissão de execução:
   ```bash
   chmod +x iac1.sh criar_user.sh
   ```

3. Execute os scripts como root:
   ```bash
   sudo ./iac1.sh
   sudo ./criar_user.sh
   ```

## 🚀 Autor

Projeto desenvolvido por **Eduardo** como parte do desafio de projeto da [DIO](https://www.dio.me/).
