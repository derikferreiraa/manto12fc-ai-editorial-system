<h1 align="center">Manto12FC — Sistema Editorial com IA</h1>
<p align="center"><strong>Dois agentes especializados. Um fluxo editorial supervisionado por pessoas.</strong></p>
<p align="center">Cultura do futebol · Pesquisa editorial · Produção de conteúdo · Design de fluxos com IA</p>
<p align="center"><a href="README.md">🇺🇸 Read in English</a></p>

## Sobre o projeto

A **Manto12FC** é um projeto independente dedicado à cultura, à memória e às histórias do futebol. Este repositório documenta um **fluxo de trabalho editorial assistido por inteligência artificial** criado para apoiar a pesquisa, a produção de textos e materiais visuais e a montagem manual das artes em templates no Canva.

O sistema é composto por **dois plugins de ChatGPT configurados separadamente**:

| Componente | Responsabilidade | Entrega |
| --- | --- | --- |
| **01 · Inteligência Editorial** | Descobrir, investigar, contextualizar e organizar pautas | Dossiês, evidências, referências visuais e ressalvas |
| **02 · Editor de Conteúdo** | Converter a pesquisa em narrativa editorial | Textos para carrosséis, roteiros de Reels/vídeos, legendas e imagens ou referências visuais, quando disponíveis |
| **Diagramação manual / Canva** | Aplicar os materiais ao template da Manto12FC | Artes finais para revisão |

> **Importante:** os agentes **não se comunicam automaticamente**. A equipe revisa o dossiê do primeiro e transfere seus insumos manualmente ao segundo. Existe **integração entre entregas**, não uma integração técnica por API ou execução automática de um agente pelo outro. Depois do Editor de Conteúdo, **a aplicação dos textos e materiais visuais ao template da Manto12FC no Canva é feita manualmente pelo criador**.

## Fluxo de produção

1. **Seleção da pauta:** definição do tema ou do recorte narrativo.
2. **Inteligência Editorial:** pesquisa de fontes, cronologia, fatos e referências visuais.
3. **Passagem manual:** curadoria humana e transferência do dossiê ao segundo agente.
4. **Editor de Conteúdo:** definição da narrativa e produção de cards, roteiros ou legendas.
5. **Montagem manual no Canva:** aplicação dos textos e das imagens ou referências do segundo agente ao template visual da Manto12FC, com ajustes de composição, tipografia e enquadramento.
6. **Revisão e publicação:** conferência factual, créditos, direitos de uso, linguagem e aprovação da arte final.

### Contrato de passagem

O primeiro agente organiza suas evidências em um contrato que facilita o uso do material pelo segundo:

- `F01`, `F02`…: **fatos e alegações**, fontes, graus de verificação e limites.
- `V01`, `V02`…: **referências visuais**, procedência, crédito e situação de direitos.
- **Ressalvas:** controvérsias, datas a confirmar e informações que não devem ser afirmadas sem comprovação.
- **Status de prontidão:** apto para redação, apto com ressalvas ou precisa de apuração.

O objetivo é preservar a qualidade da pesquisa durante a produção, evitando a perda de contexto e a reprodução de afirmações não confirmadas.

## Documentação dos agentes

**[Agente 01 — Inteligência Editorial](agents/01-editorial-intelligence.md)**: planejamento, pesquisa de atualidades, aprofundamento e investigação de fontes visuais.

**[Agente 02 — Editor de Conteúdo](agents/02-content-editor.md)**: produção dos textos e materiais de referência para carrosséis, vídeos, Reels, estáticas e legendas, com calibração editorial e validação. A montagem gráfica final acontece manualmente no Canva.

Saiba mais em [Arquitetura e passagem editorial](docs/workflow.md), [Limitações e critérios de qualidade](docs/quality-and-limits.md) e [Origem da documentação](docs/sources.md).

## Do plugin à arte no Canva

O segundo agente entrega **textos e materiais visuais**, incluindo imagens ou referências com origem identificada quando disponíveis. A partir dessa entrega, **o criador monta manualmente a publicação no Canva**, colocando os elementos em um template da Manto12FC e ajustando tipografia, enquadramento e composição. Os agentes não preenchem o template automaticamente nem exportam a arte pronta. Imagens só devem ser utilizadas depois da checagem de procedência, créditos e direitos. Veja a [etapa de produção visual](docs/canva-production.md).

## Exemplo de funcionamento

O [cenário ilustrativo sobre a estação Arsenal/Gillespie Road](examples/handoff-scenario.md) demonstra a estrutura de passagem. **Não é uma execução comprovada dos plugins nem uma matéria histórica validada.**

## Escopo técnico

- **Inteligência Editorial:** documentação baseada na versão privada `2.3.0`.
- **Editor de Conteúdo:** documentação baseada na versão privada `1.7.1`.
- **Integração:** passagem manual dos resultados, com supervisão humana.
- **Design final:** montagem manual em template no Canva.
- **Não implementado:** integração automática por API, orquestração autônoma, monitoramento contínuo, preenchimento automático de templates do Canva ou publicação automática.
- **Este repositório:** estudo de caso e documentação pública; não contém o código integral dos plugins, bases privadas ou mídia de terceiros.

**Projeto desenvolvido por Derik Ferreira para a Manto12FC**, unindo comunicação, cultura esportiva, pesquisa e aplicações de IA.

[GitHub](https://github.com/derikferreiraa) · [LinkedIn](https://www.linkedin.com/in/derikferreira/)

*Documentação de referência: novembro de 2026. Todo conteúdo passa por revisão editorial antes da publicação.*
