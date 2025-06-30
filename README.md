# multi-tenant-django

## Tipos diferentes da arquitetura Multi Tenant

1. Isolamento de Banco de Dados
    - Múltiplos tenants compartilham a mesma instância da aplicação, mas possuem bancos de dados separados

![image](https://github.com/user-attachments/assets/1987cef2-896d-4a37-bcc7-e646d62ad0b5)

2. Isolamento de schema
    - Múltiplos tenants compartilham a mesma instância da aplicação e o mesmo banco de dados, mas com esquemas diferentes
  
![image](https://github.com/user-attachments/assets/714bf8bb-be97-471d-af80-1a0b806d8208)

    
3. Isolamento de Tabela (ou compartilhado)
    - Múltiplos tenants compartilham a mesma instância da aplicação e o mesmo banco de dados, mas com tabelas diferentes

![image](https://github.com/user-attachments/assets/0a854d62-c260-48f4-8ea6-ebac3404cd97)


Isolamento de tabela (ou compartilhado), na maioria das vezes resolve o problema, além de ser o mais fácil de implementar.
Se resolve apenas com modelagem e permissões.

## Modelagem User como entidade forte (Usuário como tenant)

![image](https://github.com/user-attachments/assets/df0b49b3-11cd-414c-a314-7ac3056cb4f8)

## Modelagem Company como entidade forte (Empresa como tenant)

![image](https://github.com/user-attachments/assets/8e4ffc4b-f1c0-406a-a017-44f0d56c2041)

### Links úteis para implementação utilizando Django

- https://django-tenants.readthedocs.io/en/latest/install.html
