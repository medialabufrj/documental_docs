---
description: Documentação técnica da plataforma Documental.xyz
---

# Documental.xyz

🇬🇧 [Translate to English](https://docs-documental-xyz.translate.goog/?\_x\_tr\_sl=pt&\_x\_tr\_tl=en&\_x\_tr\_hl=en)&#x20;

🇪🇸 [Traducir para español](https://docs-documental-xyz.translate.goog/?\_x\_tr\_sl=pt&\_x\_tr\_tl=es&\_x\_tr\_hl=es)

[Documental.xyz](https://documental.xyz) é uma ferramenta para narrativas baseadas em mapas, que faz uso de recursos de _scrollytelling (interações a partir da rolagem de página)_ para navegação em dados geográficos. Ela é baseada na integração de recursos do sistema de publicação [Statamic](https://statamic.com) com o serviço de mapas online [Mapbox](https://mapbox.com).

O Documental.xyz é um complemento (um "starter kit") do Statamic e está disponível em [código aberto](https://github.com/medialabufrj/documentalxyz). Por sua vez, o Statamic é um sistema gerenciador de conteúdo (CMS) baseado no [Laravel](https://laravel.com/), um _framework_ da linguagem PHP.&#x20;

Confira abaixo um resumo do conteúdo de nossa documentação:

* [Configuração da plataforma](configuracao-da-plataforma.md): requisitos técnicos e passo a passo para instalação do Statamic;
* [Organizando os gedados no Mapbox](organizando-os-geodados-no-mapbox.md): breve tutorial sobre a organização dos dados geográficos no Mapbox e sua integração com o Statamic;
* [Publicando uma história:](publicando-uma-historia.md) breve tutorial sobre a inserção de histórias no Statamic e como chamar os geodados do Mapbox.
* [Técnicas de scrollytelling](tecnicas-de-scrollytelling.md): revisão de alternativas e tecnologias para construção de histórias com scrollytelling, para além do Documental;
* [Métodos de scrollytelling](metodos-de-scrollytelling.md): revisão de metodologias e estratégias para construção de narrativas de scrollytelling baseadas em mapas;
* [Como colaborar?](como-colaborar.md): lista de funcionalidades futuras desejáveis e informações para pessoas desenvolvedoras interessadas em colaborar com o projeto.
* [Referências e recursos](recursos-uteis.md): compilado parcial e inicial de materiais externos úteis.
* [Equipe](equipe.md): pessoas e organizações envolvidas com o Documental.

### Para quem esta documentação se destina?

Qualquer pessoa interessada pode ler a documentação sobre a ferramenta, porém, para implementar uma instância da plataforma "do zero" e publicar uma história usando os recursos do Documental, é recomendável que uma ou mais pessoas tenham conhecimentos técnicos sobre os seguintes temas:

* Noções básicas sobre a manipulação de dados geográficos;
* Configuração de servidores na web;
* Familiaridade com desenvolvimento para web e tecnologias de front-end (HTML, CSS, JavaScript);

### Preciso pagar?

O Statamic e o Mapbox adotam um modelo _freemium_, onde é possível usufruir de certas soluções com uma conta gratuita, mas é preciso assinar um serviço pago para obter recursos mais avançados. Utilizando tais recursos gratuitos ou de código aberto, qualquer pessoa pode também configurar uma instância simples da plataforma Documental.

O Documental é uma solução baseada em softwares de código aberto. Para rodar a plataforma em seu próprio computador, você pode instalar as versões gratuitas do Statamic e Mapbox, mas para publicar a plataforma em seu próprio site é necessário contratar um servidor. Na seção de [configuração da plataforma](configuracao-da-plataforma.md), é possível obter mais informações sobre os requisitos de hardware e software necessário.

As versões gratuitas do Statamic e Mapbox servem para a maioria dos casos.

| Características       | Statamic                                                                                                                          | Mapbox                                                                                                             |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Plano gratuito        | Limitado a 1 idioma e 1 usuário administrador.                                                                                    | Até 50 mil visualizações do mapa por mês.                                                                          |
| Valor do plano pago   | A partir de 259 dólares por projeto, com atualizações incluídas por um ano. Após o período, é cobrado 59 USD/ano por atualização. | Preços a partir de 50 dólares por mês ou sob demanda, a depender dos serviços utilizados ou quantidade de acessos. |
| Funcionalidades pagas | Suporte para desenvolvedores, usuários e perfis ilimitados, etc.                                                                  | Mais camadas, mais visualizações de mapas, suporte,etc.                                                            |

Para mais informações sobre os recursos pagos, confira as respectivas páginas do [Mapbox](https://www.mapbox.com/pricing) e [Statamic](https://statamic.com/pricing)

### Como creditar o projeto?

Solicitamos que projetos que façam uso da plataforma incluam a seguinte menção ao projeto, como forma de apoiar o desenvolvimento da plataforma:

`powered by Documental.xyz`

***
