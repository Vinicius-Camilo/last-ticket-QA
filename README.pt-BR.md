# Estudo de Caso de QA de Jogos: LAST TICKET

## Visão Geral

Este repositório documenta uma sessão independente de testes exploratórios de gameplay realizada em *LAST TICKET*, um jogo de terror independente desenvolvido por RayZDev.

O objetivo deste estudo de caso é demonstrar habilidades práticas em testes exploratórios, identificação de defeitos, validação de mecânicas de jogo e documentação de problemas técnicos.

- **Jogo:** [LAST TICKET](https://ray-casting.itch.io/lastticket)
- **Desenvolvedor:** RayZDev
- **Data da avaliação:** 08/07/2026
- **Versão registrada na avaliação original:** v1.0.0
- **Abordagem de teste:** Testes manuais exploratórios
- **Escopo:** Mecânicas de gameplay, interações do jogador, detecção de colisões, animações, controles e objetos do cenário

## Abordagem de Testes

Explorei as mecânicas e os ambientes do jogo, com foco em comportamentos inesperados e possíveis defeitos que pudessem afetar a experiência de jogo.

A sessão de testes abrangeu:

- Movimentação do personagem e detecção de colisões
- Mecânicas de agachamento e esconderijo
- Interação com objetos e gerenciamento de itens
- Comportamento das animações durante o gameplay
- Geometria do cenário e problemas de clipping
- Comportamento dos controles e entradas do teclado
- Progressão do jogo e evento relacionado ao ingresso
- Apresentação visual e qualidade dos textos

A gravação enviada documentou minha segunda partida. A primeira partida não foi gravada, portanto eu já conhecia parte da navegação e do funcionamento do jogo durante a sessão registrada.

## Principais Resultados

Durante a sessão, identifiquei diversos problemas que afetavam a funcionalidade e a apresentação do jogo, incluindo:

- Limites de colisão inconsistentes em objetos do cenário
- Posicionamento inesperado do personagem ao se agachar sob móveis
- Comportamento incorreto de animações durante o uso de esconderijos
- Indisponibilidade de interações durante uma sequência guiada
- Um item que podia cair para fora da área jogável em determinadas condições
- Comportamentos inesperados do personagem ao pressionar determinadas teclas
- Um evento relacionado ao ingresso que aparentemente não progrediu durante a sessão gravada

Também foram registradas observações sobre sensibilidade do mouse, elementos visuais do cenário e qualidade dos textos.

Os detalhes estão disponíveis no arquivo [Relatórios de Bugs](bug-reports.pt-BR.md).

## Resultado

O desenvolvedor forneceu um feedback positivo sobre a avaliação, destacando a identificação de bugs graves e falhas de gameplay. Também respondeu aos apontamentos e mencionou a possibilidade de um problema no gerenciamento de sequências após uma atualização.

Este estudo de caso representa os resultados de uma sessão específica de testes. Os problemas não foram retestados de forma independente em versões posteriores, portanto seu estado atual é desconhecido.

## Competências Demonstradas

- Testes manuais exploratórios
- Testes funcionais e de gameplay
- Identificação e documentação de defeitos
- Análise de problemas de colisão e animação
- Avaliação de interações do jogador
- Comunicação clara de observações técnicas
- Avaliação da experiência do usuário

## Aviso

O teste foi realizado por meio da plataforma Play2Review, que conecta desenvolvedores de jogos a testadores para a avaliação de versões de seus projetos.

Durante a atividade, realizei testes manuais exploratórios em *Last Ticket* (v1.0.0), documentando problemas de colisão, movimentação, interação com objetos e comportamento de elementos do jogo.

O feedback recebido do desenvolvedor destacou a identificação de bugs críticos e glitches. O desenvolvedor também respondeu aos relatos, mencionando a possibilidade de que uma atualização tivesse afetado o gerenciamento de sequências do jogo.

**Nota:** Os problemas descritos correspondem à versão testada e não foram verificados em versões posteriores.

Este é um estudo de caso independente de QA, baseado em uma sessão de testes de gameplay. Não se trata de um relatório oficial encomendado pelo desenvolvedor e não implica vínculo empregatício ou afiliação com o estúdio.
