# Configuração da plataforma

Statamic é um sistema gerenciador de conteúdos que pode funcionar sem um banco de dados, armazenando as informações em arquivos estáticos (_flat-file CMS_). Ele é construído como um pacote do [Laravel](https://laravel.com/), um famoso framework PHP. O Documental por sua vez é um ["starter kit" para o Statamic](https://statamic.dev/starter-kits).

## Requisitos do Statamic

O Statamic 3 requer um servidor com PHP `>= 7.4.x`. A recomendação oficial é usar pelo menos o PHP 8 com uma máquina com pelo menos 1 GB de memória RAM disponível.

Se você for configurar sua própria instância sem Docker, também é necessário instalar alguns pacotes extras o GD Library ou ImageMagick, além das seguintes extensões: BCMath, Ctype, Exif, JSON, Mbstring, OpenSSL, PDO, Tokenizer, XML.

Em um servidor Ubuntu, basta rodar o seguinte comando, [refenciado na documentação](https://statamic.dev/installing/ubuntu#install-php-amp-required-modules):

```
sudo apt install php-common php-fpm php-json php-mbstring zip unzip php-zip php-cli php-xml php-tokenizer 
```

Consulte também as instruções para instalação do [Composer](https://getcomposer.org/), gerenciador de dependências do PHP, se necessário.

Se você pretende disponibilizar a plataforma publicamente, além de um domínio na Internet, você vai precisar de um servidor. A melhor solução para o Statamic é contratar um servidor virtual privado (VPS) e a documentação oficial indica alguns serviços que facilitam o processo de _deploy_ de uma nova instância do Statamic, como o [Laravel Forge](https://forge.laravel.com/), o [Ploi.io](https://ploi.io/) ou o [ServerPilot](https://serverpilot.io/).

O site [statamic.dev/installing](https://statamic.dev/installing) lista diversas formas de instalação do Statamic, entre elas Docker, aplicação Laravel, sevidores Ubuntu ou instalações locais em Windows, MacOS ou Linux.

## Instalando o Documental no Ubuntu 20.04

Você pode usar uma solução de virtualização como o [Multipass](https://multipass.run) para rodar o seu site localmente. Confira abaixo as instruções

### Instalando dependências (PHP 8.1 e utilitários)

`sudo apt install software-properties-common`

`sudo add-apt-repository ppa:ondrej/php`

`sudo apt-get install php8.1-mbstring php8.1-xml php8.1-gd php8.1 unzip php8.1-curl`

`sudo update-alternatives --set php /usr/bin/php8.1`

### Instalando Composer

`curl -sS https://getcomposer.org/installer |php`

`sudo mv composer.phar /usr/local/bin/composer`

### Instalando Statamic CLI

`composer global require statamic/cli`

`export PATH=${PATH}:~/.config/composer/vendor/bin`

### Instalando Statamic com Documental

`statamic new documental-dev medialabufrj/documentalxyz`

Durante o processo de instalação, selecione a opção padrão ("yes") ao visualizar a pergunta:

**`Starter kit not found on Statamic Marketplace! Install unlisted starter kit? (yes/no) [yes]`**

No final do processo de instalação, crie seu usuário e senha com poderes de administração no site recém configurado.

Se tudo correu bem, você deve ver a mensagem abaixo no final.

**`"[✔] Statamic has been successfully installed into the documental-dev directory."`**

### **Rodando o Documental**

Depois da instalação, entre no diretório recém-criado (_documental-dev_) e rode o seguinte comando:

_`php artisan serve`_

Se você está usando o Multipass, adicione o parâmetro _`--host=[ip]`_ onde \[IP] é o endereço da máquina virtual (confira rodando fora da máquina virtual o comando `multipass list`).

Finalmente, acesse o navegador usando a URL com IP e a porta 8000, por exemplo:

`http://10.49.22.64:8000`

`http://127.0.0.1:8000`

Para acessar o painel de administração acesse o subdiretório **/cp** e insira as credenciais adequadas.

### **Estrutura de diretórios**

Para customizar sua instalação, será necessário alterar os arquivos nas pastas `public` e `resources`. Tenha atenção em especial aos seguintes subdiretórios:

* `public/assets/main`: localização dos arquivos enviados via upload;
* `public/css` e `public/js`: estilo e funcionalidades JavaScript do tema;
* `resources/blueprints/collections/stories`: estrutura do formulário para entrada de da dados ([blueprints](https://statamic.dev/blueprints)) das histórias;
* `resources/views`: modelo de página (template) feito com base em [Antlers](https://statamic.dev/antlers)
