# 🖱️O que é scrollytelling?

Baseado nos termos "scroll" (rolagem) e "storytelling" (contação de histórias), scrollytelling designa recursos utilizados em páginas web, onde a rolagem de tela controla a narrativa. Esta prática ganhou destaque inicial em publicações online do chamado "long form journalism" ou "jornalismo forma longa", porém, os mesmos esquemas narrativos e tecnologias também podem ser utilizados de forma mais ampla. 

A rolagem de tela é uma da formas mais intuitivas de experiência do usuário durante a utilização de dispositivos eletrônicos, sejam eles tablets, computadores desktop ou celulares. Mesmo pessoas leigas ou crianças pequenas são capazes de reproduzir este gesto em celulares, por exemplo. Com o scrollytelling, este ato simples pode controlar a aparição de textos, fotos, vídeos ou a navegação por um mapa, como implementa o Documental, além de outras possibilidades, como a transição entre diferentes formas de visualizar dados sobre um mesmo tema.

# Softwares e plataformas


## Plataformas 
Até o momento, não existem muitas opções gratuitas de plataformas que forneçam uma interface gráfica para a construção de narrativas com scrollyteling. A alternativa mais conhecida é o [Flourish.Studio](https://help.flourish.studio/article/21-controlling-stories-with-scrollytelling), que já publicou um artigo específico sobre este recurso. O Documental destaca-se por uma solução de código aberto que, a partir do Statamic e do Mapbox, fornece uma interface gráfica para controle do scrollyteling e inclusão dos conteúdos que formam a narrativa.

Existem, porém, diversas opções gratuitas ou de código aberto disponíveis atualmente para implementar páginas com recursos de *scrolytelling* "do zero". No caso do *scrollytelling*, em [artigo de janeiro de 2017](https://pudding.cool/process/how-to-implement-scrollytelling/), Russell Goldenberg elenca seis alternativas para construir uma página com scrollyteling "do zero", junto com demonstrações de seus códigos em funcionamento. A elas, foram adicionadas outras referências (entre elas a própria biblioteca mantida pelo autor, criada em outubro de 2017) e comentários próprios. As opções estão listadas de acordo com a contribuição mais recente feita em seus respectivos repositórios.

- [JEO](https://github.com/InfoAmazonia/jeo-plugin): Solução para WordPress criada pelo InfoAmazônia que permite inserir blocos de mapa interativos no editor Gutenberg.

- [Scrollama](https://github.com/russellgoldenberg/scrollama): biblioteca criada por Russel Goldenberg. Conta com uma [página com diferentes modelos prontos para uso](https://russellgoldenberg.github.io/scrollama/basic/). É uma opção relativamente acessível, mesmo para quem tem apenas conhecimentos básicos de JavaScript. O [vídeo tutorial de Jonathan Soma](https://www.youtube.com/watch?v=d7wTA9F-l8c) apresenta um bom passo a passo da implementação de uma página do tipo. Para trabalhar com mapas, vale conferir o repositório feito pelo Mapbox, com base no Scrollama. 

- [Scrollmagic](http://scrollmagic.io/): recomendada por Goldenberg para casos que exigem bastante personalização da interação. ([repositório](https://github.com/janpaepke/ScrollMagic)).

- [Scrollstory](http://sjwilliams.github.io/scrollstory/): plugin em jQuery utilizado em algumas histórias do The New York Times. É recomendado por Goldenberg para iniciantes que utilizam jQuery ([repositório](https://github.com/sjwilliams/scrollstory)).

- [graph-scroll](https://1wheel.github.io/graph-scroll/): é plugin baseado na biblioteca D3 que fornece recursos simples para scrollytelling. Recomendável especialmente para visualizações de dados que também façam uso de D3 ([repositório](https://github.com/1wheel/graph-scroll)).

O artigo de Goldenberg também cita duas bibliotecas que estão há mais tempo inativas, como o [Waypoints](http://imakewebthings.com/waypoints/), cuja última atualização do [repositório](https://github.com/imakewebthings/waypoints)é de setembro de 2016, e o [in-view.js](https://github.com/camwiegert/in-view), que está oficialmente inativo.

Além das alternativas acima, há a opção de se utilizar o [Svelte](https://svelte.dev/). Neste caso, vale a pena conferir o [modelo (template) do The Pudding](https://github.com/the-pudding/svelte-starter), que conta com um componente específico para este tipo de visualização interativa, e o [tutorial escrito por Connor Rothschild](https://www.connorrothschild.com/post/svelte-scrollytelling) mostrando como implementar scrollytelling com o Svelte.


