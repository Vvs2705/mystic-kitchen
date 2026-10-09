# Mystic Kitchen

**Estilo:** merge-2 com gestão e história, retrato.

**O que é:** você herdou uma taverna mágica abandonada e vai reconstruí-la.

**Como funciona:** geradores soltam ingredientes no tabuleiro; juntar dois iguais cria um melhor, até o prato que o cliente pediu. Os clientes pagam moedas e estrelas que reformam a taverna e liberam capítulos da história, receitas e regiões.

**Como vai ser jogar:** o prazer de juntar e ver evoluir, com a curiosidade de "o que vem depois" na cozinha e na história.

## Situação
NO-GO (merge-2 concentrado e caro em aquisição); a revisão de 2026-10-09 deixa 3 diferenciais só para o caso de reabrir. Ainda não há código: este repositório guarda o GDD e a estrutura do projeto, pronta para o desenvolvimento começar.

- **GDD:** [`docs/GDD.md`](docs/GDD.md) (revisão competitiva de 2026-10-09 no topo).
- **Comparativo com jogos similares e diferenciais:** [`docs/COMPETITIVO.md`](docs/COMPETITIVO.md).

## Estrutura do repositório
| Pasta | Para quê |
|---|---|
| `docs/` | GDD, comparativo e, depois, balance, validações e contratos de cada fase |
| `client/` | projeto Unity 6 (6000.3.x), Android primeiro, retrato; código do jogo em `client/Assets/_MK/` |
| `client/Assets/_MK/Scripts/Core/` | núcleo em C# puro (regras, simulação, save), testável fora do Unity |
| `client/Assets/_MK/Scripts/View/` | MonoBehaviours, UI, câmera, entrada |
| `client/Assets/_MK/Editor/` | setup do projeto e builds por linha de comando |
| `client/Assets/_MK/Tests/EditMode/` | testes NUnit do núcleo |
| `client/Assets/_MK/Resources/` | sprites e dados carregados em tempo de execução |
| `client/tools/` | ferramentas fora do Unity (testes `dotnet`, scripts de arte, relatório de playtest) |
| `arte/` | arte-fonte; `arte/tripo/` e `arte/mixamo/` ficam fora do git |

Como contribuir: [`CONTRIBUTING.md`](CONTRIBUTING.md). Histórico: [`CHANGELOG.md`](CHANGELOG.md).

## Repositório e licença
© V-STACK / Vinicius Souza. **Todos os direitos reservados.** Código, documentos e arte visíveis para acompanhamento, sem licença de uso, cópia ou redistribuição.
