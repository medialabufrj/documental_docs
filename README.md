---
description: Documentação técnica da plataforma Documental.xyz.
---

# 🗺 Documental.xyz

[Documental.xyz](https://documental.xyz) é uma plataforma web para narrativas baseadas em mapas, que faz uso de recursos de _scrollytelling (interações a partir da rolagem de página)_ para navegação em dados geográficos.

A ferramenta foi construída integrando recursos do sistema de publicação [Statamic](https://statamic.com) com o serviço de mapas online [Mapbox](https://mapbox.com). O primeiro é um sistema gerenciador de conteúdo (CMS) construído como um pacote do Laravel, um framework da linguagem PHP.

![](.gitbook/assets/stack\_docxyz.png)

Ambos os serviços adotam um modelo _freemium_, onde é possível usufruir de recursos básicos com uma conta gratuita, mas é preciso assinar um serviço pago para obter recursos mais avançados. Utilizando tais recursos gratuitos ou de código aberto, qualquer pessoa pode também configurar uma instância simples da plataforma Documental.

Nesta documentação, veremos como é possível configurar uma instância do site “do zero” e como publicar seus primeiros mapas.

### Preciso pagar?

O Documental é uma solução baseada em softwares de código aberto. Para rodar a plataforma em seu próprio computador, você pode instalar as versões gratuitas do Statamic e Mapbox, mas para publicar a plataforma em seu próprio site é necessário contratar um servidor. Na seção de [configuração da plataforma](configuracao-da-plataforma.md), é possível obter mais informações sobre os requisitos de hardware e software necessário.

As versões gratuitas do Statamic e Mapbox servem para a maioria dos casos.

| Características       | Statamic                                                                                                                          | Mapbox                                                                                                             |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Plano gratuito        | Limitado a 1 idioma e 1 usuário administrador.                                                                                    | Até 50 mil visualizações do mapa por mês.                                                                          |
| Valor do plano pago   | A partir de 259 dólares por projeto, com atualizações incluídas por um ano. Após o período, é cobrado 59 USD/ano por atualização. | Preços a partir de 50 dólares por mês ou sob demanda, a depender dos serviços utilizados ou quantidade de acessos. |
| Funcionalidades pagas | Suporte para desenvolvedores, usuários e perfis ilimitados, etc.                                                                  | Mais camadas, mais visualizações de mapas, suporte,etc.                                                            |

Para mais informações sobre os recursos pagos, confira as respectivas páginas do [Mapbox](https://www.mapbox.com/pricing) e [Statamic](https://statamic.com/pricing)

### Para quem esta documentação se destina?

Qualquer pessoa interessada pode ler a documentação sobre a ferramenta, porém, para implementar uma instância da plataforma "do zero", é recomendável conhecimentos técnicos sobre os seguintes temas:

* Noções básicas sobre a manipulação de dados geográficos;
* Configuração de servidores na web;
* Familiaridade com desenvolvimento para web e tecnologias de front-end (HTML, CSS, JavaScript);

### Créditos

Solicitamos que projetos que façam uso da plataforma incluam uma menção ao projeto, como forma de apoiar o desenvolvimento da plataforma.

**Coordenação**

[Agência Autônoma](https://autonoma.xyz)

[Medialab/UFRJ](https://medialabufrj.net)

#### Desenvolvimento de software

[Marlus Araújo](https://github.com/sulram) (versão inicial)

Rafael Bantu (atualização e publicação do add-on e tema)

#### Documentação

[Adriano Belisario](https://github.com/belisards)

****
