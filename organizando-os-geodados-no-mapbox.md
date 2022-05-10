# Organizando os geodados no Mapbox

Antes de iniciar o trabalho com o Mapbox, vale a pena relembrar algumas boas práticas ao trabalhar com dados geográficos, que irão ajudar no desenvolvimento do seu projeto.

* Adote um padrão consistente para nomear os arquivos geográficos;
* Crie uma pasta diferente para cada fonte de dado;
* Se possível, padronize o formato e a projeção dos geodados.&#x20;

Atualmente, o Mapbox Studio aceita o formatos GeoTIFF para arquivos em malha (raster) e diversos outros para dados vetoriais (MBTiles, KML, GPX, GeoJSON, Shapefile zipado ou tabelas CSV). Neste segundo caso, recomendamos especialmente o uso do formato GeoJSON, ao invés do tradicional Shapefile, para usos na web. Você pode usar uma solução online e de código aberto como o [Mapshaper](https://mapshaper.org) para fazer a conversão de formatos facilmente.

Se você já organizou seus dados localmente e criou uma conta no [Mapbox](https://www.mapbox.com), vá até o Mapbox Studio, que é como um “Photoshop para mapas”, segundo o site oficial da empresa. Para começar, crie um estilo novo e, caso queira, selecione um modelo básico com imagem de satélite ou cartografias.&#x20;

Na customização deste novo estilo, iremos enviar os geodados por meio do ícone de adição do lado esquerdo da tela, na opção ‘COMPONENTS’, selecionando a opção ‘DATA VISUALIZATION’ e em seguida ‘UPLOAD DATA’

Para conectar o Statamic na sua conta do Mapbox, você irá precisar destas duas informações:

**Mapbox** **Style**: um caminho do estilo criado no sistema do Mapbox. Por exemplo: ‘_mapbox://styles/seu\_usuario\_aqui/cdas81aito3zbk2sfs5vb1tfm6_’

**Mapbox Access Token**: é uma longa sequência aleatória de caracteres, que serve como senha para acessar seus dados no Mapbox.
