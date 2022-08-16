# 🔧 Configuração da plataforma

Statamic é um sistema gerenciador de conteúdos que pode funcionar sem um banco de dados, armazenando as informações em arquivos estáticos (_flat-file CMS_). Ele é construído como um pacote do [Laravel](https://laravel.com/), um famoso framework PHP. O Documental por sua vez é um ["starter kit" para o Statamic](https://statamic.dev/starter-kits).

## Requisitos do Statamic

O Statamic 3 requer um servidor com PHP `>= 7.4.x`. A recomendação oficial é usar pelo menos o PHP 8 com uma máquina com pelo menos 1 GB de memória RAM disponível.

Se você for configurar sua própria instância sem Docker, também é necessário instalar alguns pacotes extras o GD Library ou ImageMagick, além das seguintes extensões: BCMath, Ctype, Exif, JSON, Mbstring, OpenSSL, PDO, Tokenizer, XML.&#x20;

Consulte também as instruções para instalação do [Composer](https://getcomposer.org/), gerenciador de dependências do PHP, se necessário.

Se você pretende disponibilizar a plataforma publicamente, além de um domínio na Internet, você vai precisar de um servidor. A melhor solução para o Statamic é contratar um servidor virtual privado (VPS) e a documentação oficial indica alguns serviços que facilitam o processo de _deploy_ de uma nova instância do Statamic, como o [Laravel Forge](https://forge.laravel.com/), o [Ploi.io](https://ploi.io/) ou o [ServerPilot](https://serverpilot.io/).

O site [statamic.dev/installing](https://statamic.dev/installing) lista diversas formas de instalação do Statamic, entre elas Docker, aplicação Laravel, sevidores Ubuntu ou instalações locais em Windows, MacOS ou Linux.&#x20;



## Instalando o Documental no Ubuntu 20.04

### Instalando dependências (PHP 8.1 e utilitários)

`sudo apt install software-properties-common`&#x20;

`sudo add-apt-repository ppa:ondrej/php`&#x20;

`sudo apt-get install php8.1-mbstring php8.1-xml php8.1-gd php8.1 unzip php8.1-curl`&#x20;

`sudo update-alternatives --set php /usr/bin/php8.1`

### Instalando Composer

`curl -sS https://getcomposer.org/installer |php`&#x20;

`sudo mv composer.phar /usr/local/bin/composer`

### Instalando Statamic CLI

`composer global require statamic/cli`&#x20;

`export PATH=${PATH}:~/.config/composer/vendor/bin`

### Instalando Statamic com Documental

`statamic new documental-dev rafaelbantu/documental`
