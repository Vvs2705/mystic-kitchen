# MYSTIC KITCHEN

## Game Design Document — Versão de Produto

> **Revisão 2026-10-09 (comparativo de mercado):** comparativo com fontes, matriz de recursos e o teste de 6 ângulos em [COMPETITIVO.md](COMPETITIVO.md). Conclusão honesta: **não encontrei ângulo viável que tire este jogo do "mais um merge" para um estúdio do nosso tamanho, e o NO-GO de 2026-10-06 se mantém** (§44).
> - O porquê, em uma linha: a receita do merge-2 vem exatamente do que os jogadores reclamam (energia, escada de gems, eventos de pressão). Tirar isso derruba o LTV que paga a UA; manter nos torna um clone sem orçamento. E 0 de 91 lançamentos do H1/2025 passou de US$100 mil por mês.
> - O tema não diferencia: o Tasty Travels (culinária, US$127 milhões líquidos no H1/2026) é o 2º do gênero, e a líder Microfun já tem um merge de culinária (Flambé).
> - A energia do §15 (100, +1 a cada 2 min) é idêntica à do Gossip Harbor, inclusive na reclamação que ela gera. Ficou anotada no §15, com a regra do MVP da raia B.
> - Correções da validação feitas dentro das seções: Android primeiro (§1); "Borin" virou "Dorvo" (§10); 1 moeda no MVP (§16); baús de conteúdo fixo (§24, §25, §27); guildas e Cloud Save marcados como dependentes de backend (§28, §40); guardrails de monetização (§29, §31).
> - Seções novas no fim: veredito competitivo (§44), diferenciais caso o jogo seja reaberto (§45) e KPIs numéricos, kill criteria e MVP de 3 semanas (§46), que o GDD não tinha.
> - Nota desta revisão (opinião, sem dado de jogador): design 6 → 6,5 (o documento ganhou números e gates); mercado 4 → 3 (a pesquisa achou o merge de culinária da líder e a taxa de 0 em 91 lançamentos).

### 1. VISÃO DO PRODUTO

**Nome provisório:** Mystic Kitchen

**Gênero:** Merge-2 + Management + Narrative + Collection

**Plataforma primária:** Android / iOS *(revisão 2026-10-09: Android primeiro, como o resto do portfólio; iOS só depois de validar)*

**Orientação:** Portrait

**Modelo:** Free-to-Play

**Monetização:** IAP + Rewarded Ads + eventos + passe sazonal

**Público principal:** jogadores de casual/merge, aproximadamente 25–55 anos, com forte potencial para público interessado em culinária, fantasia, decoração e progressão.

**Fantasia central:**

O jogador herdou uma pequena taverna mágica abandonada e precisa reconstruí-la até transformá-la no maior restaurante fantástico do reino.

Não administramos apenas uma cozinha.

Descobrimos ingredientes mágicos, receitas perdidas, clientes misteriosos e novas regiões.

---

# 2. PITCH

Combine ingredientes mágicos, prepare pratos extraordinários e reconstrua uma antiga taverna enquanto descobre os segredos culinários de um mundo fantástico.

Cada novo cliente, região e receita expande tanto o tabuleiro de Merge quanto a história e a economia do restaurante.

---

# 3. PILARES DO PRODUTO

## Pilar 1 — Merge satisfatório

Arrastar dois objetos iguais precisa produzir feedback extremamente prazeroso.

Som.

Partículas.

Animação.

Haptic.

Progressão visual clara.

---

## Pilar 2 — Descoberta

O jogador deve constantemente pensar:

**“O que vem depois?”**

Isso vale para:

- cadeia de Merge;
- receitas;
- clientes;
- regiões;
- criaturas;
- restaurantes;
- segredos;
- coleções.

---

## Pilar 3 — Construção

O Merge gera recursos.

Os recursos transformam visualmente o mundo.

A taverna precisa evoluir de um prédio abandonado para um estabelecimento fantástico.

---

## Pilar 4 — Narrativa leve

A narrativa dá propósito à progressão sem interromper constantemente o gameplay.

---

## Pilar 5 — Mundo expansível

Precisamos poder lançar novas regiões durante anos sem alterar o sistema central.

---

# 4. CORE LOOP

O loop principal será:

**Gerar ingredientes**

→

**Merge**

→

**Criar ingredientes superiores**

→

**Preparar pedidos**

→

**Atender clientes**

→

**Ganhar moedas, estrelas e recursos**

→

**Reformar restaurante**

→

**Liberar história, novas receitas e generators**

→

**Voltar ao Merge.**

---

# 5. LOOP DE SESSÃO

Uma sessão típica de 4–12 minutos:

1. jogador abre o jogo;
2. coleta recompensa offline;
3. verifica pedidos;
4. utiliza energia;
5. gera itens;
6. faz merges;
7. completa alguns pedidos;
8. recebe moedas/XP;
9. melhora restaurante;
10. coleta eventos;
11. realiza missão diária;
12. encerra sessão.

Algumas horas depois, energia e generators recuperaram capacidade.

O jogador retorna.

---

# 6. TABULEIRO PRINCIPAL

Grid inicial:

**7 × 9**

Expansível progressivamente.

Parte dos espaços começa bloqueada.

Desbloquear espaço é uma progressão importante.

Categorias de objetos:

### Ingredientes

Vegetais.

Carnes.

Peixes.

Frutas.

Temperos.

Grãos.

Ingredientes mágicos.

### Utensílios

Panelas.

Fornos.

Caldeirões.

Facas.

Pratos.

### Pratos

Sopa.

Pão.

Ensopado.

Sobremesa.

Poções culinárias.

Pratos mágicos.

---

# 7. GENERATORS

Generators criam itens iniciais em troca de energia.

Exemplos:

### Cesta da Fazenda

Produz:

grãos;

vegetais;

ervas.

### Caixa do Pescador

Produz:

peixes;

mariscos;

algas.

### Jardim Encantado

Produz:

ervas mágicas;

cogumelos;

flores.

### Despensa

Produz:

farinha;

açúcar;

temperos.

### Caldeirão Arcano

Produz ingredientes mágicos raros.

Generators também possuem níveis.

Exemplo:

**Cesta Nv.1**

↓

Cesta Nv.2

↓

Horta

↓

Horta Encantada

↓

Fazenda Real.

Generators superiores:

produzem itens melhores;

possuem menor cooldown;

podem gerar itens raros.

---

# 8. CADEIAS DE MERGE

Uma cadeia exemplo:

Trigo

→

Feixe de trigo

→

Farinha

→

Massa

→

Pão

→

Pão temperado

→

Pão encantado.

Outra:

Peixe pequeno

→

Peixe fresco

→

Filé

→

Peixe assado

→

Banquete marítimo

→

Banquete do Leviatã.

As cadeias não precisam sempre representar transformações literais.

Prioridade:

legibilidade e satisfação.

---

# 9. SISTEMA DE RECEITAS

Receitas funcionam como coleção permanente.

Cada prato possui:

nome;

raridade;

região;

ingredientes;

descrição;

ilustração.

Categorias:

Comum

Raro

Épico

Lendário

Mítico.

Receitas descobertas entram no:

**Grimório Culinário.**

Completar páginas oferece recompensas.

---

# 10. CLIENTES

Clientes possuem personalidade.

Exemplos:

### Dorvo

*(Revisão 2026-10-09: o nome era "Borin", que colide com o NPC ferreiro do COE.)*

Anão minerador.

Prefere carnes e cervejas mágicas.

### Elowen

Elfa botânica.

Prefere ingredientes naturais.

### Mira

Feiticeira.

Solicita receitas raras.

### Grub

Goblin comerciante.

Pede comida estranha e paga muito.

### Sir Aldric

Cavaleiro.

Introduz missões de aventura.

Clientes recorrentes criam vínculo.

Quanto mais são atendidos:

amizade aumenta;

novos pedidos aparecem;

histórias são desbloqueadas;

recompensas exclusivas surgem.

---

# 11. SISTEMA DE REPUTAÇÃO

O restaurante possui nível de reputação.

Pedidos completados geram:

⭐ Reputação.

Exemplo:

Nível 1 — Barraca esquecida.

Nível 5 — Taverna local.

Nível 15 — Restaurante regional.

Nível 30 — Taverna famosa.

Nível 50 — Restaurante Real.

Nível 75 — Santuário Culinário.

Nível 100 — Cozinha Lendária.

Não deve haver nível máximo rígido.

---

# 12. RESTAURAÇÃO

Cada capítulo possui um espaço visual.

Exemplo inicial:

**Taverna Abandonada**

Jogador restaura:

entrada;

mesas;

balcão;

forno;

jardim;

andar superior;

salão principal;

cozinha;

área externa.

Cada melhoria gera transformação visual significativa.

Algumas decisões de decoração podem ser oferecidas entre três opções.

A escolha é cosmética.

---

# 13. REGIÕES

O jogo não termina quando a primeira taverna é concluída.

Ela é apenas o capítulo inicial.

## Região 1 — Bosque de Mosswood

Tema:

fantasia medieval verde.

Introduz:

fazenda;

ervas;

cogumelos.

## Região 2 — Emberpeak

Vulcânica.

Introduz:

temperos;

carnes;

ingredientes de fogo.

## Região 3 — Frosthaven

Neve.

Introduz:

peixes;

raízes;

ingredientes congelados.

## Região 4 — Sunscar Desert

Deserto fantástico.

Introduz:

frutas;

especiarias;

criaturas exóticas.

## Região 5 — Celestial Isles

Ilhas voadoras.

Introduz ingredientes mágicos avançados.

Novas regiões podem continuar indefinidamente.

---

# 14. META PROGRESSION

Temos cinco eixos simultâneos:

### 1. Player Level

Desbloqueia sistemas.

### 2. Restaurant Level

Representa a expansão física.

### 3. Recipe Collection

Progressão de coleção.

### 4. Character Relationships

Progressão narrativa.

### 5. World Exploration

Progressão territorial.

Isso impede que o jogador dependa de uma única barra de progresso.

---

# 15. ENERGIA

Energia máxima inicial:

100.

Produção:

1 energia aproximadamente a cada 2 minutos.

Custos:

generator normalmente consome 1 energia por geração.

Fontes adicionais:

level up;

daily reward;

rewarded ads;

missões;

eventos;

IAP.

O design deve evitar sensação de bloqueio constante.

Energia existe para:

regular sessões;

criar motivo de retorno;

dar valor a recompensas;

viabilizar monetização.

### Revisão 2026-10-09 — energia

- **Os números deste § são os mesmos do líder.** O Gossip Harbor usa energia máxima de 100 e +1 a cada 2 min (3h20 para encher), e é exatamente disso que os reviews mais reclamam, junto com a compra de energia em escada de gems que reseta todo dia (fontes no COMPETITIVO.md).
- **A conta da raia B:** um item de tier 6 sai de 2⁵ = 32 gerações, então um tanque cheio cobre uns 3 pedidos altos. A "1ª hora" do §20 consome várias vezes 100 de energia. Sem refill por level-up, a parede aparece já na sessão 1. "Evitar bloqueio" e "energia viabiliza monetização" se contradizem: neste gênero, a energia *é* o bloqueio.
- **Regra para o MVP, se o jogo for reaberto (raia B):** energia só é cobrada a partir do nível 5 do jogador e enche no level-up. A alternativa a testar é não ter energia nenhuma (M2, §45).

---

# 16. ECONOMIA

Principais currencies:

### Gold

Soft currency.

Usado para:

melhorias;

loja;

alguns desbloqueios.

### Gems

Hard currency.

Usado para:

energia;

slots;

cooldown;

itens especiais.

### Stars

Progressão narrativa.

Obtidas principalmente através de pedidos.

Usadas para reformas.

### Event Currency

Moeda temporária de evento.

### Revisão 2026-10-09 — moedas

Guardrail do portfólio: **1 moeda no MVP** (Estrelas, que pagam a restauração). Gold, Gems e Event Currency só entram quando houver ralo no mapa de fontes e ralos. O offline nunca concede gems nem moeda de evento, e toda recompensa leva id de transação.

---

# 17. PEDIDOS

Tipos:

### Pedido rápido

Fácil.

Boa frequência.

### Pedido complexo

Itens avançados.

Maior recompensa.

### Pedido de personagem

Avança relacionamento.

### Pedido narrativo

Avança história.

### Pedido especial

Tempo limitado.

### Pedido de evento

Usa itens sazonais.

O board nunca deve ficar dominado por pedidos impossíveis.

---

# 18. SISTEMA DE PEDIDOS DINÂMICOS

O jogo deverá observar:

nível do jogador;

generators;

espaço disponível;

estoque atual;

histórico recente.

O sistema evita gerar constantemente pedidos muito distantes.

Também podemos utilizar Remote Config para ajustar pesos.

---

# 19. INVENTÁRIO

Jogador possui:

board;

storage.

Storage começa limitado.

Slots adicionais podem ser:

comprados com moedas;

desbloqueados;

comprados com gems.

Storage é também um sink econômico importante.

---

# 20. D1 — PRIMEIRO DIA

Objetivos:

ensinar Merge;

apresentar taverna;

introduzir narrativa;

introduzir generators;

completar primeira reforma;

entregar primeiro momento de descoberta.

Até aproximadamente a primeira hora acumulada o jogador deverá conhecer:

Merge;

pedidos;

energia;

reforma;

receitas;

personagem principal;

coleção.

---

# 21. D7

Jogador provavelmente terá:

vários generators;

primeiro grande salão restaurado;

10–20 receitas;

3–5 personagens;

eventos disponíveis;

missões diárias;

recompensa semanal.

---

# 22. D30

Jogador:

terminou ou está avançado na primeira região;

possui vários generators evoluídos;

coleciona receitas raras;

participa de eventos;

entende economia;

possivelmente fez primeira compra.

Nesse ponto começa transição para progressão de longo prazo.

---

# 23. D90+

Conteúdo passa a ser sustentado por:

novas regiões;

eventos;

novos personagens;

coleções;

generators;

temporadas;

histórias especiais.

---

# 24. DAILY SYSTEM

Todo dia:

3–5 Daily Quests.

Exemplos:

merge 50 itens;

complete cinco pedidos;

gaste 40 energia;

complete um pedido raro.

Completar todas fornece:

Daily Chest (revisão 2026-10-09: conteúdo fixo e mostrado antes de abrir; nada de sorteio).

---

# 25. WEEKLY SYSTEM

Sete dias de progresso acumulativo.

Recompensa final:

baú premium (revisão 2026-10-09: conteúdo fixo e visível; ECA Digital, art. 20);

energia;

gems;

item raro.

---

# 26. EVENTOS

### Festival Gastronômico

Board independente.

7 dias.

Receitas exclusivas.

### Banquete Real

Complete pedidos especiais.

### Caçada aos Ingredientes

Colete tokens durante gameplay normal.

### Jornada do Chef

Progressão linear estilo battle pass.

### Mercado Místico

Loja temporária.

### Chef's Challenge

Sequência de objetivos progressivamente difíceis.

---

# 27. TEMPORADAS

Duração:

aproximadamente 28 dias.

Season Pass com:

trilha gratuita;

trilha premium.

Conteúdo:

energia;

gems;

baús;

decorações;

avatar;

receita especial.

Evitar vantagens permanentes excessivas.

*Revisão 2026-10-09:* os baús do passe têm conteúdo fixo e visível. Nenhum produto pago, nem moeda comprada, leva a sorteio.

---

# 28. SOCIAL

Social não será obrigatório no lançamento.

Fase posterior:

Guildas culinárias.

Jogadores contribuem para:

banquetes;

eventos cooperativos;

metas semanais.

Não haverá multiplayer em tempo real.

*Revisão 2026-10-09:* guildas e eventos cooperativos pressupõem backend, e o MVP do portfólio não tem backend. Ficam fora de qualquer versão até existir um.

---

# 29. MONETIZAÇÃO

Prioridade:

IAP.

Rewarded Ads complementares.

## IAP

Starter Pack.

Pacotes de gems.

Pacote de energia.

Event Bundle.

Season Pass.

Generator Bundle.

Storage Bundle.

## Rewarded Ads

Opções:

energia;

bubble item;

redução de cooldown;

refresh de pedido;

recompensa adicional.

Interstitial obrigatório deve ser evitado ou muito limitado em um Merge de maior LTV.

*Revisão 2026-10-09 (guardrails do portfólio):* interstitial desligado na v0.1; nada de item aleatório pago (ECA Digital, Lei 15.211/2025, art. 20); boosters pagos desligados em qualquer ranking; recompensa com id de transação. A validação apontou que pôr IAP como prioridade num gênero de LTV tardio exige retenção acima do hybrid-casual (ver §46).

---

# 30. PRIMEIRA COMPRA

Starter Pack precisa oferecer valor extremamente visível.

Exemplo:

gems;

energia;

um baú;

slot adicional;

decoração exclusiva.

Preço de entrada baixo.

---

# 31. BUBBLE SYSTEM

Após alguns merges, item adicional pode aparecer em bolha.

Jogador pode:

usar gems;

assistir rewarded ad;

ignorar.

Sistema deve possuir limite de frequência.

*Revisão 2026-10-09:* se reaberto, a bolha abre só por rewarded, nunca por gems (M5, §45). Bolha paga somada a storage pago e tabuleiro apertado vira venda de alívio de entupimento (raia B).

---

# 32. LIVE OPS

Calendário ideal:

segunda — nova missão semanal;

terça — mini-evento;

quinta — evento principal;

sexta a domingo — bonificação;

mensal — temporada;

trimestral — nova região ou feature.

---

# 33. CONTEÚDO DE LANÇAMENTO

Objetivo comercial inicial:

1 região completa.

1 restaurante.

aproximadamente 150–250 pedidos preparados.

30–50 receitas.

10–15 cadeias de Merge.

6–8 generators.

6 personagens principais.

3 tipos de eventos.

Daily + Weekly.

Season system preparado tecnicamente.

Isso deverá proporcionar dezenas de horas distribuídas ao longo de várias semanas.

---

# 34. ARTE

Estilo:

3D estilizado ou 2.5D.

Referência visual:

fantasia amigável.

Formas arredondadas.

Materiais simples.

Personagens expressivos.

Itens precisam ser extremamente legíveis em telas pequenas.

Cadeias de Merge devem possuir silhuetas progressivamente mais impressionantes.

---

# 35. ÁUDIO

Cada Merge:

feedback curto.

Merge avançado:

som progressivamente mais gratificante.

Outros sons importantes:

pedido concluído;

baú;

moedas;

gem;

level up;

reforma;

recipe discovery.

Música:

fantasia aconchegante.

---

# 36. ARQUITETURA UNITY

Sistemas principais:

GameManager

MergeBoardManager

GridManager

ItemDatabase

ItemFactory

GeneratorSystem

OrderManager

CharacterManager

NarrativeManager

EconomyManager

EnergyManager

InventoryManager

RecipeCollectionManager

QuestManager

EventManager

SeasonManager

SaveManager

CloudSaveManager

RemoteConfigManager

AnalyticsManager

AdsManager

IAPManager

AudioManager

NotificationManager.

Conteúdo deverá ser majoritariamente data-driven usando ScriptableObjects e/ou backend/configuração remota.

---

# 37. ANALYTICS

Eventos fundamentais:

session_start

session_end

tutorial_step

item_generated

item_merged

order_completed

order_abandoned

energy_spent

energy_received

currency_source

currency_sink

restaurant_upgrade

recipe_unlocked

character_level

event_start

event_complete

rewarded_offer

rewarded_complete

shop_open

iap_offer_view

iap_purchase.

---

# 38. KPIs DE PRODUTO

Monitorar:

tutorial completion;

D1;

D3;

D7;

D30;

sessions per DAU;

session length;

energy spent/day;

orders/day;

merge count/session;

event participation;

rewarded opt-in;

payer conversion;

ARPDAU;

ARPPU;

LTV;

CPI.

Benchmarks externos devem ser tratados como referência, nunca meta automática.

*Revisão 2026-10-09:* as metas numéricas e os kill criteria que faltavam estão no §46.

---

# 39. UA — MARKETABILITY

Criativos devem comunicar o jogo em segundos.

Possíveis hooks:

“Qual ingrediente vem depois?”

“Você consegue completar este pedido?”

“Ela herdou a pior taverna do reino.”

“Combine dois itens e veja no que se transformam.”

“Do barraco ao melhor restaurante do reino.”

Também podemos testar criativos de falha intencional.

*Revisão 2026-10-09:* a raia A julgou estes hooks genéricos do gênero (diferencial em 3 s: NÃO). O único hook novo que vale testar é "um merge que não manda você esperar" (M2), contra o controle, em amostra Tier-1 (§46).

---

# 40. ROADMAP

## MVP

Merge.

Generator.

Pedidos.

Economia.

Energia.

Primeiras reformas.

Analytics.

## Alpha

30+ receitas.

narrativa.

personagens.

daily missions.

monetização básica.

## Soft Launch

Região completa.

Eventos.

IAP.

Ads.

Remote Config.

Cloud Save.

*Revisão 2026-10-09:* Cloud Save e Remote Config remoto pressupõem backend, fora do padrão do portfólio para o MVP.

## 1.0

Season.

coleções.

live ops calendar.

pipeline de conteúdo.

## Pós-lançamento

Nova região aproximadamente a cada 8–12 semanas inicialmente.

Após pipeline maduro, cadência pode aumentar.

---

# 41. EXPANSÃO DE ANO 1

Q1:

lançamento + otimização.

Q2:

segunda região.

Guild beta.

novos eventos.

Q3:

terceira região.

coleções especiais.

eventos cooperativos.

Q4:

quarta região.

sistema social mais profundo.

eventos sazonais.

---

# 42. RISCOS

### Conteúdo caro

Mitigação:

reutilizar sistemas e assets.

### Board frustrante

Mitigação:

telemetria para identificar falta de espaço e pedidos excessivos.

### Energia agressiva

Mitigação:

equilibrar recompensas gratuitas.

### História cara

Mitigação:

narrativa curta e modular.

### Tema excessivamente genérico

Mitigação:

criar identidade forte dos personagens, receitas e mundo.

### Mercado concentrado (revisão 2026-10-09)

Mitigação: nenhuma disponível para o nosso tamanho. A Microfun tem ~55% do merge-2 e um merge de culinária próprio, e 0 de 91 lançamentos do H1/2025 passou de US$100 mil por mês. Ver §44.

### Público e ECA Digital (revisão 2026-10-09)

Mitigação: nenhum item aleatório pago, por construção (§16, §24, §25, §27).

---

# 43. VISÃO DE LONGO PRAZO

Mystic Kitchen não termina quando restauramos a cozinha.

O produto deve poder crescer através de:

novos continentes;

novos restaurantes;

centenas de receitas;

novos chefs;

guildas;

coleções;

temporadas;

eventos;

novas cadeias de Merge.

O objetivo é construir um **Merge live-service com universo culinário próprio**, e não uma campanha descartável.

---

# 44. VEREDITO COMPETITIVO (revisão 2026-10-09)

**Conclusão: não existe ângulo viável que tire o Mystic Kitchen do "mais um merge" para um estúdio do nosso tamanho. O NO-GO se mantém.** Detalhe, fontes e matriz em [COMPETITIVO.md](COMPETITIVO.md).

**Os 6 ângulos testados** (existe? aparece em 3 s? paga a UA? cabe no time?):

| Ângulo | Por que não fecha |
|---|---|
| A. Merge sem energia | Existe em jogos pequenos e na Netflix (Diner Out). Sem venda de energia não há LTV para pagar UA no Tier-1 |
| B. Narrativa profunda | Love & Pies, Gossip Harbor e Merge Mansion já fazem, e é o conteúdo mais caro para um dev solo |
| C. Culinária como sistema | Flambé (Microfun) e Tasty Travels já ocupam o tema; melhora o core, mas não posiciona |
| D. Monetização justa | Não aparece em criativo e corta a receita que paga a aquisição |
| E. Premium ou assinatura | Depende de contrato com a plataforma, fora do nosso modelo F2P Android |
| F. Merge-puzzle de níveis fechados | Fecha nas 4 perguntas, mas é **outro jogo** e disputa o slot de puzzle com Rune Relay e Skyhold |

**Os 4 motivos, em ordem de peso:**
1. A receita do merge-2 vem do que os jogadores reclamam (energia, escada de gems, eventos de pressão). Tirar derruba o LTV (US$4,7 por download no H1/2025); manter nos torna um clone sem orçamento de UA.
2. O que seria diferente (tabuleiro justo, preço honesto) é invisível num criativo de 3 s.
3. O espaço está fechado: a Microfun tem ~55% do merge-2 e um merge de culinária próprio; o 2º colocado é de culinária (Tasty Travels, US$127 milhões líquidos no H1/2026); 0 de 91 lançamentos do H1/2025 passou de US$100 mil/mês.
4. O gênero vive de cadência de conteúdo (eventos semanais, regiões a cada 8–12 semanas, §40), que um dev solo não sustenta.

**Recomendação:** arquivar este GDD como referência. Não gastar com criativos agora. Duas peças podem ser reaproveitadas em outros jogos do portfólio: o gerador de pedidos com garantia de solução (M1, §45) e, se o Rune Relay validar, a ideia de níveis fechados com tema de cozinha (M6) como candidata futura ao slot de puzzle.

**O que reabriria o jogo:** um publisher ou plataforma de assinatura interessado no tema (ângulo E), ou o ângulo F aprovado como jogo próprio depois do resultado de coorte do Rune Relay. As duas decisões são do Vinicius.

---

# 45. DIFERENCIAIS COMPETITIVOS (se o jogo for reaberto) (revisão 2026-10-09)

Resumo; o detalhe está no [COMPETITIVO.md](COMPETITIVO.md), seção (e). Custo: P ≤ 1 semana · M 2–4 semanas · G ≥ 1 mês. Todos são PROPOSTA. **Nenhum muda o veredito do §44:** eles melhoram o jogo, mas não criam rota de aquisição.

| # | Diferencial | Responde a | Custo | Ordem |
|---|---|---|---|---|
| M2 | Sem energia: o ritmo vem da carga do gerador, do forno e do espaço | Parede de energia (Gossip Harbor, Travel Town) | P | **1º, só como teste de criativo** |
| M1 | Tabuleiro que nunca entope: pedido só aparece se o solver provar que é resolvível | Tabuleiro cheio, tarefa que leva dias (Travel Town, Merge Mansion) | M | **2º** (reaproveitável no portfólio) |
| M6 | Modo de níveis fechados com solução única (pivot do ângulo F) | Falta de diferencial em 3 s | M protótipo / G jogo | **3º, só como pergunta de portfólio** |
| M3 | Escolha de receita no pedido (rápida × caprichada) | Core sem decisão (raia B) | M | se reaberto |
| M4 | Narrativa no balcão, nunca em pop-up bloqueante | História dispersa (Merge Mansion) | M | se reaberto |
| M5 | Oferta honesta: preço fixo, sem bolha paga, sem aleatório pago | Escada de gems que reseta (Gossip Harbor) | P | se reaberto |

---

# 46. KPIs NUMÉRICOS, KILL CRITERIA E MVP DE 3 SEMANAS (revisão 2026-10-09)

O GDD original só listava nomes de métricas (§38) e não tinha kill criteria (validação, raia D). Esta seção vale **apenas se o jogo for reaberto**.

**Gate 0, antes de qualquer código:**
- 8 criativos, incluindo "um merge que não manda você esperar" (M2) e o criativo de controle (dois itens viram um melhor).
- Amostra pequena em Tier-1 (EUA/CA) além de BR, porque install barato em BR/PH/ID não prova merge, que monetiza no Tier-1 (raia A).
- O GDD não define CPI-alvo, e esta pesquisa não achou CPI de merge Tier-1 verificado. Por isso o Gate 0 é relativo: **o M2 precisa superar o controle em IPM em ≥20% em 2 famílias de criativo**. Se não superar, o jogo fica arquivado.

**Metas de retenção (as duas réguas valem):**
- **Piso do portfólio (veredito):** D1 ≥26%, D7 ≥5%, coorte de 1,5–2k installs, cancelar só depois de 2 iterações.
- **Barra do merge (raia B):** D1 ≥28%, D7 ≥6%. O merge precisa reter mais que o hybrid-casual porque o LTV vem de IAP tardio.
- Entre o piso e a barra, o jogo não escala UA. Abaixo do piso depois de 2 iterações, cancela.
- Payer conversion só é lida a partir de 5k installs.

**Kill criteria:**
- **K1 Retenção:** D1 <26% ou D7 <5% depois de 2 iterações → cancelar.
- **K2 Energia/ritmo (raia B):** >40% dos jogadores que esgotam energia (ou carga dos geradores, se M2) na sessão 1 não voltam no D1, **ou** a mediana dos retidos fica abaixo de 3 sessões por dia.
- **K3 Custo (raia B):** uma cadeia nova (6–8 itens de arte + balance) leva mais de 3 dias-dev, **ou** os pedidos não podem ser gerados por regra → cancelar, independentemente dos KPIs.
- **K4 Tabuleiro (M1):** >10% das sessões com tabuleiro >90% cheio por mais de 60 s → o gerador de pedidos falhou; corrigir antes de qualquer leitura de retenção.

**MVP de 3 semanas (proposta da raia B):**
- **Entra:** tabuleiro 7×9 e 2 geradores; 2 cadeias × 6 tiers (12 itens); 3 pedidos visíveis, nunca mais de 2 tiers acima do que está no tabuleiro; energia cobrada só a partir do nível 5 do jogador e enchendo no level-up (ou M2, sem energia); 1 cômodo de restauração com 6 tarefas pagas em estrelas; 1 personagem estático; 1 moeda (Estrelas).
- **Fica fora:** narrativa, os outros clientes, regiões, grimório, eventos, temporada, gems e IAP, storage pago, bolhas, cloud save e guildas.
- **Telemetria mínima:** `order_generated` (com o resultado do solver), `board_fill_pct`, `energy_depleted` (ou `generator_empty`), `session_start/end`, `order_completed` com id de transação.
