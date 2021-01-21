# Configurando o IPtables via Ansible 

## Sobre :star:

Utilizando o ansible para realizar configurações de acesso no IPtables. 

## Recursos utilizados :page_facing_up:

* Configurações validadas no Ubuntu 16.x e 18.04 LTS
* Ansible [v2.9.10](https://docs.ansible.com/ansible/2.9/installation_guide/intro_installation.html)
* Módulo [IPtables](https://docs.ansible.com/ansible/2.9/modules/iptables_module.html)

## Execução e ações :rocket:

O arquivo main.yml está estruturado para executar os seguintes passos:
* Garantir que o IPtables e o Python estejam instalados nos alvos.
* Executar um flush na chain configurada.
* Criar as entradas personalizadas dos respectivos alvos.
* Criar entradas padrões nos alvos, essas regras entrem por último.
* Salva as alterações.
