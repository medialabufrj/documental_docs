---
description: Documentação técnica da plataforma Documental.xyz.
---

# Documental.xyz

[Documental.xyz](https://documental.xyz) é uma plataforma web para narrativas baseadas em mapas, que faz uso de _scrollytelling_ para navegação em dados geográficos.&#x20;

A ferramenta foi construído integrando recursos do sistema de publicação [Statamic](https://statamic.com) com o serviço de mapas online [Mapbox](https://mapbox.com). Ambos os serviços adotam um modelo _freemium_, onde é possível usufruir de recursos básicos com uma conta gratuita, mas é preciso assinar um serviço para obter recursos mais avançados. Utilizando tais recursos gratuitos ou de código aberto, qualquer pessoa pode também configurar uma instância simples da plataforma Documental.&#x20;

Nesta documentação, veremos como é possível uma instância do site “do zero”, em um servidor auto-hospedado.

### Para quem esta documentação se destina?

Qualquer pessoa interessada pode ler a documentação sobre a ferramenta, porém, para implementar uma instância da plataforma "do zero", é recomendável conhecimentos técnicos sobre os seguintes temas:

* Noções básicas sobre a manipulação de dados geográficos;&#x20;
* Configuração de servidores na web;
* Familiaridade com desenvolvimento para web e tecnologias de front-end (HTML, CSS, JavaScript);&#x20;

### Planos gratuitos vs pagos

|                       | Statamic                                                                                                                          | Mapbox                                                                                                             |
| --------------------- | --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Plano gratuito        | Limitado a 1 idioma e 1 usuário administrador                                                                                     | Até 50 mil visualizações do mapa por mês.                                                                          |
| Valor do plano pago   | A partir de 259 dólares por projeto, com atualizações incluídas por um ano. Após o período, é cobrado 59 USD/ano por atualização. | Preços a partir de 50 dólares por mês ou sob demanda, a depender dos serviços utilizados ou quantidade de acessos. |
| Funcionalidades pagas | Suporte para desenvolvedores, multi-idioma, usuários e perfis ilimitados, etc.                                                    | Mais camadas, mais visualizações de mapas, suporte,etc.                                                            |

#### Fontes

[Mapbox pricing](https://www.mapbox.com/pricing)

[Statamic pricing](https://statamic.com/pricing)
