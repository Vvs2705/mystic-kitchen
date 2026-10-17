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

---

## Lições do estúdio aplicadas a Mystic Kitchen (do Dungeon Courier, 2026-10-16)

O Dungeon Courier (DC) chegou à 1.4.1-beta com o GDD inteiro feito, arte v2, tutorial guiado, anúncios e compras integrados e AAB assinado. O que lá custou tempo, crédito ou retrabalho virou o playbook do estúdio: [LICOES_PARA_O_ESTUDIO.md](https://github.com/Vvs2705/dungeon-courier/blob/main/docs/LICOES_PARA_O_ESTUDIO.md), com cópia na memória do estúdio em `C:\Users\VINICIUS\Videos\MEUS PROJETOS\Agentes\_memoria\PLAYBOOK_ESTUDIO_DUNGEON_COURIER.md`. Esta seção traduz as lições para o Mystic Kitchen, e é PROPOSTA. **O NO-GO do §44 continua valendo:** a seção serve agora para a peça que o §44 manda reaproveitar (o gerador de pedidos com solver, M1) e, se o jogo for reaberto, para o MVP de 3 semanas do §46. Nada aqui justifica gastar crédito nem abrir o projeto Unity antes de uma decisão do Vinicius. Notação: `DC:` = repositório `Vvs2705/dungeon-courier`; `Forge:` = `Vvs2705/forge-street`. Os clipes Mixamo ficam fora do git, no disco do estúdio: `JOGOS NOVOS\06_DUNGEON_COURIER\arte\mixamo\` (DC), `JOGOS NOVOS\03_FORGE_STREET\arte\mixamo\` (Forge) e `ARKANA\mobile-unity\Assets\_Arkana\Resources\mixamo-*.fbx` (ARKANA). O reuso entre projetos tem aval do Vinicius de 2026-10-09 (`DC:docs/PROVENIENCIA.md` §3).

### Processo

- **Contrato do Gate 0 e do MVP antes de qualquer código.**
  - **Fazer:** se o jogo for reaberto, o 1º documento é `docs/CONTRATO_GATE0.md`, só de mídia: 8 criativos, e o M2 precisa superar o controle em IPM em ≥ 20% em 2 famílias de criativo (§46). O 2º é `docs/CONTRATO_MVP.md`, copiado do "Entra / Fica fora" do §46 com os números (7×9, 2 geradores, 2 cadeias × 6 tiers, 3 pedidos visíveis, nunca mais de 2 tiers acima). A matriz "GDD × feito" lista **todas** as 46 seções; as do "Fica fora" entram como "fora por decisão do §46", não como "falta".
  - **Por quê:** no DC, o contrato escrito antes deixou núcleo e View andarem em paralelo. Aqui ele protege o escopo: o GDD descreve um live-service (§26–§28, §32, §41) e 24 sistemas, quase todos managers (§36), e sem a matriz isso volta pela porta dos fundos.
  - **Reaproveitar:** `DC:docs/CONTRATO_V01.md` e `DC:docs/CONTRATO_LANCAMENTO.md` §1 (matriz) e §10 ("fica de fora por decisão do próprio GDD").
- **Memória de retomada:** `_memoria\STATUS_mystic-kitchen.md`, com o bloco "CONTINUAR DAQUI", só quando houver trabalho. Hoje o bloco diria: "arquivado; reabre pelo ângulo E ou F do §44".
- **Livro-razão de créditos e fotos antes do PR,** como no DC (`DC:docs/PROVENIENCIA.md` §1–§2). No DC, as fotos acharam defeitos de tela que 169 testes verdes não viam.

### Código e testes

- **Núcleo C# puro: tabuleiro, merge, geradores, pedidos e solver.**
  - **Fazer:** em `Scripts/Core`, com passo fixo, xorshift com semente e o `Sim` como fachada:
    - `Board`: 7×9, com células bloqueadas;
    - `MergeChain`: a cadeia em dados;
    - `Generator`: carga e recarga, para o M2;
    - `OrderGenerator` + `Solver`: o M1. Só emite pedido resolvível com o espaço livre e no máximo 2 tiers acima do que há no tabuleiro; acima de 85% de ocupação, o pedido consome o que já está lá.

    A View só desenha e lê os eventos.
  - **Por quê:** o solver é a peça que o próprio §44 quer reaproveitar no portfólio. Em C# puro, ele roda em `dotnet test` e serve a qualquer jogo com fila de clientes.
  - **Reaproveitar:** o esqueleto do DC (`Core/` + `Sim.cs` + `client/tools/coretests` + `client/tools/viewcheck`). O `client/README.md` deste repo já prevê esse layout.
- **Invariantes viram testes nomeados:**
  - `Pedido_SempreResolvivel`: o solver prova antes de mostrar;
  - `Pedido_NoMaximo2TiersAcima`;
  - `Tabuleiro_SempreTemSaida`: sempre há um merge, uma venda ou um pedido que consome;
  - `Recompensa_Idempotente`: id de transação (§16);
  - `GeradorVazio_NaoTravaPedidoRapido`.
  - **Por quê:** no DC, regra que ficou só em prosa não sobreviveu ao código; teste nomeado sobreviveu.
- **Bot e `-autoplay N` medem o K2 e o K4.**
  - **Fazer:** o bot joga 1 000 sessões (o "validar barato" do M1 no `COMPETITIVO.md`) e imprime `board_fill_pct`, o tempo com o tabuleiro acima de 90%, os pedidos por sessão, as gerações até o tier 6 (a conta de 2⁵ = 32 do §15) e as estrelas por hora. O resultado vai para `docs/BALANCE.md`.
  - **Reaproveitar:** `DC:client/Assets/_DC/Scripts/Core/Bot.cs`; `Forge:client/tools/econsim/`.
- **Validador de cadeias e receitas fora do Unity.**
  - **Fazer:** uma tabela em `docs/`, checada por um `client/tools/cadeias_check.py --selftest`. Ele confere: ids únicos; toda receita usa itens que algum gerador produz; cada cadeia tem 6–8 tiers; nomes em inglês e espanhol com ≤ 16 caracteres. É a parte de dados do K3 ("cadeia nova em ≤ 3 dias-dev").
  - **Reaproveitar:** `Forge:client/tools/conteudo_check.py`. O Forge tem receitas e produtos no mesmo formato.
- **Diário CSV de playtest** com a telemetria mínima do §46 (`order_generated` com o resultado do solver, `board_fill_pct`, `generator_empty`, `order_completed` com id de transação), antes de qualquer SDK. **Reaproveitar:** `DC:client/Assets/_DC/Scripts/View/Exportar.cs` e `DC:client/tools/diario_report.py`.
- **Flags de teste**, todas só com `-testsession` (não lê nem grava save, semente 1):
  - as do DC: `-tela tabuleiro|restauracao|grimorio`, `-bot`, `-lang`, `-shot`, `-record` e `-tutorial`;
  - uma nova, `-board <arquivo>`, que carrega um tabuleiro de teste para fotografar o estado "quase cheio" do K4.
- **Portão de todo PR**, igual ao do DC: `dotnet test` · `viewcheck` · Unity EditMode · build Windows · `-autoplay 30` sem exceção · fotos 540×960.
- **Áudio sintetizado, com tom por tier.**
  - **Fazer:** o "som progressivamente mais gratificante" do §35 sai de graça de um script: o mesmo som de merge, com altura e brilho subindo a cada tier. Haptic leve no merge, como o DC faz ao pousar e pegar a carga.
  - **Reaproveitar:** `DC:client/tools/audio_gen.py` (determinístico, com semente pelo nome do som).

### Arte e animação

- **Os itens do tabuleiro são ícones, e é aí que o crédito não precisa entrar.**
  - **Fazer:** pinte cada cadeia **numa folha só** do gerador grátis (Nano Banana 2), em grade e sobre azul-marinho liso, e corte por célula com `ui_assets.py`. Exemplo: Trigo → Pão encantado, os 7 tiers do §8. A folha única mantém o estilo entre os tiers. A silhueta crescente que o §34 pede se confere numa folha de contato, com a silhueta preta a 64 px, para caçar pares confundíveis. Alternativa, também a 0 crédito: modelar por primitivas no Blender, como os produtos do Forge.
  - **Por quê:** no DC, 20 ícones numa folha 4×3 saíram consistentes e de graça. O 3D do Tripo, a 45 créditos por item, estoura o K3 em cadeias de 12 a 100+ ícones.
  - **Reaproveitar:** `DC:client/tools/ui_assets.py`; `Forge:client/tools/itens_blender.py` e `folha_produtos.py`.
- **Variantes por troca de cor.**
  - **Fazer:** os níveis de gerador (Cesta Nv.1 → Nv.2), o "temperado" e o "encantado" de cada cadeia e as versões regionais (peixe de Frosthaven, tempero de Emberpeak) saem do mesmo ícone com `roupas_cor.recolor` mais brilho, a 0 crédito.
  - **Atenção:** o ícone recolorido não pode se confundir com outro tier; ele também passa pela folha de silhuetas.
  - **Reaproveitar:** `DC:client/tools/roupas_cor.py`.
- **Clientes: retrato pintado antes de 3D.**
  - **Fazer:** o MVP do §46 tem 1 personagem estático: um retrato pintado no gerador grátis, no estilo do logo, com 3 expressões (pedindo, esperando, satisfeito). Os 5 clientes do §10 só ganham corpo 3D se a restauração (§12) precisar deles andando no salão.
  - **Por quê:** no DC, o retrato pintado ficou muito mais vistoso que o render 3D recortado, e o cartão do cliente virou a cena de contexto.
- **Se os clientes ganharem corpo** (depois de reaberto, com aval por lote): Tripo HD (45) + Auto Rig Mixamo (20) = 65 cada, ou 325 pelos 5. O item fica sempre separado e preso ao osso pelo `--attach` do `DC:client/tools/render_sprites.py`. Clipes que já existem:

  | Quem | Item separado | Clipes |
  |---|---|---|
  | todos | — | parado: Forge `Idle.fbx` (Breathing Idle); andar até o balcão: ARKANA `mixamo-loc-andar-frente.fbx`; chegar: Forge `Waving.fbx`; esperar: Forge `LookingAround.fbx`; pedido entregue: Forge `Thankful.fbx` e `Cheering.fbx`; "não tem?": DC `_blender/Shrug.fbx` |
  | Dorvo | caneca e picareta | segurar a caneca: DC `_blender/Hold.fbx`; o brinde é clipe novo no `DC:client/tools/anim_blender.py` |
  | Elowen | cesta de ervas | DC `_blender/Hold.fbx` |
  | Mira | cajado | ARKANA `mixamo-standing-1h-cast-spell-01.fbx`, ou DC `_blender/NecroIdle.fbx` e `NecroCast.fbx` (feitos para o cajado ficar em pé na mão) |
  | Grub | saco | DC `_blender/Hold.fbx` e `Grab.fbx`; jogar a moeda no balcão: DC `_blender/KoboldToss.fbx`; o tamanho do saco se ajusta a 0 crédito como no `DC:client/tools/saco_ladrao.py` |
  | Sir Aldric | espada e escudo | DC `_blender/GuardIdle.fbx` e `Bash.fbx`; ARKANA `mixamo-standing-block-idle.fbx` |
  | chef (se tiver corpo) | colher, panela | mexer o caldeirão e provar: clipes novos no Blender, 0 crédito |

- **Restauração (§12) a 0 crédito.**
  - **Fazer:** o "antes e depois" de mesa, balcão e forno sai do mesmo prop: no gerador grátis, com o mesmo prompt nas versões "quebrada" e "restaurada"; ou modelado por primitivas e deformado no Blender. Props do Tripo (45 cada) só para as peças-âncora do salão.
  - **Por quê:** o baú que abre e a planta de boca aberta do DC saíram de um modelo só, sem geração nova.
  - **Reaproveitar:** `Forge:client/tools/props_blender.py`; `DC:client/tools/bau_abrindo.py` e `planta_aberta.py`.
- **Arte de interface pintada:** logo; ícones da HUD (estrelas, gerador, loja, grimório, configurações) numa folha 4×3; fundo da taverna abandonada e da restaurada; retratos dos clientes. **Custo de Tripo no MVP: 0.**

### Interface e marca

- **Moldura sem PNG.** A moldura de madeira com rebites do DC serve direto à taverna. O `Pergaminho` vira o cartão de pedido e a página do Grimório (§9); o `Balao` é a fala no balcão (M4); o `Contorno` destaca a célula do tutorial. **Reaproveitar:** `DC:client/Assets/_DC/Scripts/View/Art.cs`.
- **Fontes OFL,** com a licença junto, em `Resources/Fonts`.
- **Legibilidade do tabuleiro.** O 7×9 em 1080 de largura dá ~140 px por célula. O alvo de 48 dp (`Dp.cs`) cabe por pouco, e o ícone precisa ler a 64 px; por isso existe a folha de silhuetas.
- **Telas 20:9.** A sobra de altura mostra o salão da taverna (o balcão com o cliente), nunca uma faixa lisa. No DC, a faixa lisa parecia bug.
- **Ícone adaptativo.** Um prato-símbolo ou o caldeirão, ocupando no máximo 0,64 da camada e conferido nas 3 máscaras. **Reaproveitar:** `DC:client/tools/icone_app.py`.

### Onboarding

- **Cartão de contexto no lugar de cutscene.**
  - **Fazer:** "herdou uma taverna abandonada" não precisa de abertura animada. O 1º cliente, Dorvo, entra em retrato pintado, com balão: *"Essa taverna abriu de novo? Faz anos que ninguém serve um pão decente em Mosswood. Me arruma um pão e eu pago em estrelas."* O ciclo fecha quando ele volta na 1ª reforma.
  - **Reaproveitar:** o `Passo.Fala` de `DC:client/Assets/_DC/Scripts/View/Tour.cs`.
- **Tutorial guiado (coach marks).** Cada passo aparece uma vez só, com Pular e REVER TUTORIAL; fica desligado no `-testsession`. Nos passos de ação, só o alvo aceso responde.

  | # | Quando | O que | Por quê |
  |---|---|---|---|
  | 1 | logo após o cartão | tocar na Cesta da Fazenda (só ela acesa); sai um trigo | o gerador é a fonte de tudo |
  | 2 | em seguida | tocar de novo: 2º trigo | o merge precisa de dois iguais |
  | 3 | em seguida | arrastar trigo sobre trigo (dedo animado do `Arrastar`): vira feixe | é o verbo central e vem antes de qualquer escolha |
  | 4 | em seguida | repetir até o pão; sem cartão novo, só o contorno na próxima dupla | mostra "o que vem depois" (Pilar 2) sem parede de texto |
  | 5 | pão pronto | arrastar o pão até o pedido do Dorvo | fecha o loop pedido → estrela |
  | 6 | 1ª estrela | 1ª tarefa de restauração: a mesa da entrada (botão aceso) | estrela vira taverna (Pilar 3) |
  | 7 | 1º gerador vazio | explicação: "a cesta descansa e volta em X min; enquanto isso, junte o que já tem" | com o M2, é o único limite; com energia (só a partir do nível 5, §15), o texto muda. Nunca vender recarga neste passo |
  | 8 | 1º `board_fill_pct` > 85% | explicação: vender ou guardar | é o K4: ensina a saída antes da frustração |

  - Os passos 7 e 8 leem o estado do núcleo, como os gatilhos do DC, e não o relógio.
  - Passo de ação se cancela se a tela mudar: no DC, um passo preso sem alvo congelou o jogo.
- **Nada tampando o alvo.** O item arrastado sobe ~1 dedo acima do toque, para a célula de destino ficar visível. O jogo não tem joystick; no DC, o controle desenhado no dedo tampava o personagem.

### Monetização e compliance

- **O que se copia do DC:**
  - 1 moeda (Estrelas), offline de 2 h, rewarded opcional e interstitial desligado;
  - anúncio não personalizado e sem `AD_ID`. Para o público de 25–55 anos, a configuração do DC serve: GDPR sem consentimento, CCPA opt-out, COPPA desligado;
  - IAP atrás de uma interface, com loja falsa no PC e compra em 2 passos;
  - política de privacidade no GitHub Pages.
  - **Reaproveitar:** `DC:client/Assets/_DC/Scripts/View/Anuncios.cs`, `AnunciosLevelPlay.cs`, `Loja.cs`, `LojaIap.cs` e `DC:docs/MONETIZACAO.md` §4.
- **O que o GDD original contraria** está nos conflitos 1–3 abaixo, e esses conflitos pesam mais que qualquer reaproveitamento.

### Play e lançamento

- **Conta de organização.** O D-U-N-S é da V-STACK, não do jogo: use a mesma conta de organização que o DC está abrindo, sem pedir outro D-U-N-S.
- **Identidade do app.** appId `br.com.vstack.mystickitchen`; chave de upload em `%USERPROFILE%\.mystickitchen\`, fora do git e com backup fora do PC; AAB pelo `Setup.BuildAndroidBundle`.
- **Loja e criativos:** `loja_fotos.sh`, `loja_assets.py` e `criativos.py`, todos em `DC:client/tools/`. O criativo de controle ("dois itens viram um melhor") e o do M2 saem de um build gravado com `-record`.

### Android

- **Taxa de quadros.** `vSyncCount = 0` e `targetFrameRate = 60` logo no início: a animação de merge é o Pilar 1, e 60 fps faz parte do "feedback prazeroso".
- **Build.** APK de worktree só via `subst R:`, e só o APK atual fica no disco.
- **Desempenho** se mede em aparelho original. Ferramenta: `Forge:client/tools/medir_aparelho.sh`.

### Conflitos com o GDD atual

1. **Energia comprável + gerador que solta item raro = sorteio pago indireto (§7, §15, §16, §29).**
   - **O problema:** "Generators superiores podem gerar itens raros" (§7), somado à energia vendida por gems e por IAP (§15, §16 e o "Pacote de energia" e o "Generator Bundle" do §29), faz o dinheiro comprar tentativas de um resultado aleatório. Esse é o "indiretamente" que o Beast Haven escreveu na regra do §28 dele, à luz do art. 20 do ECA Digital (a leitura jurídica final é do Vinicius).
   - **Recomendação:** adotar o M2 (sem energia), ou energia que nunca se vende. O item raro do gerador sai por contador visível ("a cada 10 gerações, 1 raro"), não por probabilidade.
2. **Raridade de receita, de Comum a Mítico (§9), e o "item raro" do baú semanal (§25).** Se algum caminho pago leva ao raro, volta o problema 1. **Recomendação:** raridade por receita conhecida (como a receita de habitat do Beast Haven), nunca por drop.
3. **Storage pago com gems (§19), bolha (§31) e tabuleiro apertado.** O GDD já marcou a bolha; o storage pago completa a "venda de alívio de entupimento". **Recomendação:** no MVP, storage só por progresso ou por estrelas.
4. **Arquitetura de 24 sistemas, quase todos managers (§36).** Contraria o núcleo puro com fachada única do DC e o `client/README.md` deste repo: manager MonoBehaviour não roda em `dotnet test`. **Recomendação:** `Core/` com o `Sim` e sistemas puros; `CloudSaveManager` e `RemoteConfigManager` ficam fora, porque dependem de backend (o §40 já diz isso).
5. **Gate 0 com criativos "antes de qualquer código" (§46) × a regra "criativo só do jogo real".** **Recomendação:** 1 semana de tabuleiro mínimo (gerador, merge e 1 pedido, com arte do gerador grátis), gravado com `-record`; só então o teste de IPM.
6. **Arte "3D estilizado ou 2.5D" (§34).** Num jogo de ícones e retratos, o 3D gasta crédito sem ganho legível a 64 px. **Recomendação:** ícones e retratos pintados (0 crédito); 3D só se a restauração pedir personagens andando.
7. **Live-service (§26–§28, §32, §41) para um dev solo.** O DC conseguiu fechar o GDD inteiro porque o conteúdo era finito e estava contratado; regiões a cada 8–12 semanas não cabem. Isso já está no veredito do §44. Fica registrado que nenhuma ferramenta do DC muda essa conta: elas baixam o custo por cadeia, não a cadência exigida.

### Primeiros passos recomendados

1. Manter o NO-GO do §44: nenhuma geração com crédito e nenhum projeto Unity sem decisão do Vinicius.
2. Já agora, extrair o M1 como peça de portfólio: especificar `OrderGenerator` + `Solver` em C# puro, com os testes nomeados acima, num repositório que já tenha `coretests`. É o reaproveitamento que o §44 recomenda.
3. Se o jogo for reaberto: escrever `docs/CONTRATO_GATE0.md` e `docs/CONTRATO_MVP.md` a partir do §46, com a matriz GDD × feito marcando as seções "fora por decisão".
4. Decidir no GDD os conflitos 1–3 (energia, raro e storage) antes de qualquer criativo, porque eles mudam o que o vídeo pode mostrar.
5. Pintar no gerador grátis a folha das 2 cadeias do MVP (12 itens) e adaptar o `folha_produtos.py` para a checagem de silhuetas; 0 crédito.
6. Copiar o esqueleto do DC (`Setup.cs`, `coretests`, `viewcheck`, `Art.cs`, `Tour.cs` e `Textos.cs`) e fazer o núcleo do tabuleiro com o bot medindo o K4.
7. Gravar o build mínimo com `-record`, montar os criativos com `criativos.py` e só então rodar o Gate 0 de IPM.
