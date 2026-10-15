# Relatórios de Bugs — LAST TICKET

**Data dos testes:** 08/07/2026  
**Método de teste:** Testes manuais exploratórios  
**Jogo:** [LAST TICKET](https://ray-casting.itch.io/lastticket)  
**Versão registrada na avaliação original:** v1.0.0

Estes relatórios resumem os problemas observados durante uma sessão de testes exploratórios. Os passos de reprodução são apresentados somente quando sustentados pelas observações originais. Os problemas não foram retestados de forma independente em versões posteriores.

## 1. Colisões do Personagem e Geometria do Cenário

### BUG-001 — O personagem consegue atravessar mesas do escritório

**Categoria:** Detecção de colisões

**Comportamento observado:** O personagem conseguia atravessar as mesas do escritório, com exceção da mesa de Maya.

**Comportamento esperado:** Objetos sólidos do cenário devem impedir consistentemente a passagem do personagem, salvo quando esse comportamento for intencional.

**Notas de reprodução:** Tentar caminhar contra as mesas do escritório. O comportamento não era consistente entre todas elas.

### BUG-002 — O personagem consegue atravessar objetos do cenário

**Categoria:** Detecção de colisões

**Comportamento observado:** O personagem conseguia atravessar uma planta e um barril localizados do lado de fora do escritório.

**Comportamento esperado:** Objetos que deveriam ocupar um espaço físico sólido devem possuir limites de colisão adequados.

### BUG-003 — Agachar-se sob uma mesa causa clipping e reposicionamento inesperado

**Categoria:** Movimentação do personagem / Colisões

**Comportamento observado:** Ao se agachar sob a mesa do escritório, o personagem parecia atravessar visualmente o móvel. Ao tentar se levantar enquanto permanecia embaixo dele, o personagem era reposicionado sobre a mesa ou ao lado dela.

**Comportamento esperado:** A movimentação deve respeitar a geometria dos móveis e evitar reposicionamentos não intencionais.

### BUG-004 — Abrir o portão pode prender o personagem

**Categoria:** Colisões / Geometria do cenário

**Comportamento observado:** Ao se posicionar diretamente abaixo do portão acima da entrada do escritório e abri-lo, o personagem ficava preso. Fechar o portão ou se afastar agachado permitia voltar a se movimentar.

**Comportamento esperado:** A abertura do portão não deve prender o personagem em uma situação não intencional.

## 2. Mecânicas de Esconderijo e Animações

### BUG-005 — O estado de agachamento persiste após entrar em um armário

**Categoria:** Estado do personagem / Mecânicas de gameplay

**Comportamento observado:** Após se agachar para entrar em um armário, o personagem permanecia agachado. Ainda era possível se levantar e, em algumas ocasiões, voltar a se agachar.

**Comportamento esperado:** A postura do personagem e os estados relacionados ao esconderijo devem ser atualizados consistentemente ao entrar e sair do armário.

### BUG-006 — A animação de movimento da cabeça continua dentro do armário

**Categoria:** Animações

**Comportamento observado:** Ao entrar em um armário enquanto estava em movimento, a animação de oscilação da cabeça às vezes continuava sendo reproduzida enquanto o personagem estava escondido.

**Comportamento esperado:** As animações devem corresponder ao estado atual do personagem e não continuar quando forem incompatíveis com o estado de esconderijo.

## 3. Interação com Objetos e Gerenciamento de Itens

### BUG-007 — Interações com objetos ficam indisponíveis durante uma sequência guiada

**Categoria:** Interações / Progressão de gameplay

**Comportamento observado:** Durante a sequência em que o NPC "Maya" apresentava o ambiente ao jogador, não era possível interagir com os objetos. As portas continuavam interativas.

**Comportamento esperado:** As interações devem permanecer disponíveis quando isso for previsto pela sequência atual do jogo.

### BUG-008 — Um item descartado pode cair para fora da área jogável

**Categoria:** Gerenciamento de itens / Limites do cenário

**Comportamento observado:** O jogador conseguia descartar um objeto enquanto estava dentro de um armário. Ao olhar novamente para dentro do armário e descartar o objeto, ele caía para fora da área jogável.

**Comportamento esperado:** Itens descartados devem permanecer acessíveis dentro do ambiente jogável ou seguir as regras previstas para o gerenciamento de itens.

## 4. Entradas e Controles

### BUG-009 — Pressionar a tecla T interrompe a movimentação do personagem

**Categoria:** Tratamento de entradas

**Comportamento observado:** Pressionar a tecla T interrompia completamente a movimentação do personagem durante a sessão.

**Comportamento esperado:** A movimentação do personagem não deve ser interrompida por uma entrada sem função aparente para o jogador.

**Observações:** A causa não foi determinada. O comportamento pode justificar uma investigação sobre os mapeamentos de teclas e o gerenciamento de estados do jogo.

### OBS-001 — Alterações inesperadas de velocidade ao usar as teclas de mais e menos

**Categoria:** Entradas / Controles

**Comportamento observado:** Pressionar as teclas de mais e menos aparentemente alterava a velocidade do jogo.

**Comportamento esperado:** Caso essas teclas não sejam controles destinados ao jogador, elas não devem alterar inesperadamente o gameplay.

**Observações:** A causa não foi confirmada.

### OBS-002 — A sensibilidade do mouse continua alta na configuração mínima

**Categoria:** Controles / Configurações

**Comportamento observado:** A sensibilidade do mouse continuava alta demais para um controle confortável, mesmo quando configurada no nível mínimo.

**Comportamento esperado:** A configuração mínima deve proporcionar uma redução perceptível da sensibilidade.

## 5. Progressão do Gameplay

### OBS-003 — O evento relacionado ao ingresso aparentemente não progride

**Categoria:** Progressão de gameplay / Gerenciamento de eventos

**Comportamento observado:** Durante as duas sessões, o evento de "chegada do ticket" esperado não aconteceu, apesar do tempo de espera. A gravação de gameplay incluía esse período.

**Comportamento esperado:** O evento relacionado à "chegada do ticket" deve ocorrer quando as condições necessárias de progressão forem atendidas.

**Observações:** As condições exatas de ativação e o tempo de espera esperado não foram determinados durante a sessão. A observação não confirma, por si só, a causa subjacente.

## 6. Qualidade Visual e Textual

### OBS-004 — O calendário apresenta problemas visuais e textuais perceptíveis

**Categoria:** Qualidade visual

**Comportamento observado:** O calendário do escritório apresentava inconsistências visuais perceptíveis e aparentes erros.

**Comportamento esperado:** Os elementos visuais do cenário devem atender ao padrão de qualidade esperado e evitar inconsistências que prejudiquem a imersão.

### OBS-005 — Problemas gramaticais em diálogos

**Categoria:** Qualidade textual / Localização

**Comportamento observado:** Foram identificados problemas gramaticais em alguns trechos, principalmente em um diálogo do NPC relacionado à cópia de vozes.

**Comportamento esperado:** Os textos do jogo devem ser gramaticalmente corretos e consistentes com o significado pretendido.

## Resumo

A sessão identificou problemas em diferentes áreas, incluindo detecção de colisões, mecânicas de esconderijo, interação com objetos, tratamento de entradas, progressão de gameplay e apresentação.

Os resultados foram compartilhados com o desenvolvedor por meio da avaliação original. Não há confirmação, neste relatório, sobre o estado desses problemas em versões posteriores.
