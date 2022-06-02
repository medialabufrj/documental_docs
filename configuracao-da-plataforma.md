# 🔧 Configuração da plataforma

Statamic é um sistema gerenciador de conteúdos que pode funcionar sem um banco de dados, armazenando as informações em arquivos estáticos (_flat-file CMS_). Ele é construído como um pacote do [Laravel](https://laravel.com/), um famoso framework PHP.

## Requisitos do Statamic

O Statamic 3 requer um servidor com PHP `>= 7.4.x`. A recomendação oficial é usar pelo menos o PHP 8 com uma máquina com pelo menos 1 GB de memória RAM disponível.

O site [statamic.dev/installing](https://statamic.dev/installing) lista diversas formas de instalação do Statamic, entre elas Docker, aplicação Laravel, sevidores Ubuntu ou instalações locais em Windows, MacOS ou Linux.

Se você for configurar sua própria instância sem Docker, também é necessário instalar alguns pacotes extras o GD Library ou ImageMagick, além das seguintes extensões: BCMath, Ctype, Exif, JSON, Mbstring, OpenSSL, PDO, Tokenizer, XML. Em um servidor Ubuntu, basta rodar o seguinte comando, [refenciado na documentação](https://statamic.dev/installing/ubuntu#install-php-amp-required-modules):

```
sudo apt install -y php-common php-fpm php-json php-mbstring zip unzip php-zip php-cli php-xml php-tokenizer 
```

Consulte também as instruções para instalação do [Composer](https://getcomposer.org/), gerenciador de dependências do PHP.

### Configurando um servidor na web

Se você pretende disponibilizar a plataforma publicamente, além de um domínio na Internet, você vai precisar de um servidor. A melhor solução para o Statamic é contrar algum VPS (servidor virtual privado) e a documentação oficial indica alguns serviços que facilitam o processo de _deploy_ de uma nova instância do Statamic, como o [Laravel Forge](https://forge.laravel.com/), o [Ploi.io](https://ploi.io/) ou o [ServerPilot](https://serverpilot.io/)
