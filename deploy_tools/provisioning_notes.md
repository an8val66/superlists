Provisionamento de um novo site
===============================

## Pacotes necessários:

* nginx
* python ^3.6
* virtualenv + pip
* git

Por exemplo, no Ubuntu:

    sudo apt update
    sudo apt install nginx python3 python3-venv git

## Config do Nginx Virtual Host

* veja nginx.template.conf
* substitua SITENAME, por exemplo, por staging.tonepo.com.br

## Servico Systemd

* veja gunicorn-systemd.template.service
* substitua SITENAME, por exemplo, por staging.tonepo.com.br

## Estrutura de pastas:
Suponha que temos uma conta de usuário em /home/username

/home/username
----sites
    ----SITENAME
        ----database
        ----source
        ----static
        ----venv