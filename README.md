# T-Intervalos para a web

Recriação do aplicativo educativo T-Intervalos a partir do pacote Windows `T-Intervalos-Deploy4.zip`, com análise REA do código, configurações e recursos originais.

## Modos

- **Tom e Semitom:** reconheça distâncias de um ou dois semitons.
- **Classificação Básica:** identifique o número do intervalo pela grafia das notas.
- **Classificação Completa:** escolha primeiro o número e depois a qualidade; somente a resposta completa contabiliza acerto.
- **Auditivo:** reconheça intervalos pelo som, em quatro conjuntos de respostas.

São 30 fases em quatro dificuldades (Elementar, Fácil, Médio, Difícil), com tempo, meta, limite de erros consecutivos e desbloqueio por perfil. A prática permite intervalos ascendentes, descendentes, harmônicos ou mistos; simples e compostos; contexto cromático ou diatônico; tonalidades e claves Sol/Fá/Dó.

Os nove capítulos de fundamentos usam os textos e diagramas originais. O capítulo de apoio instrumental inclui dez exemplos originais de piano e violão.

## Executar

Node.js 20 ou superior. Sem dependências para instalar:

```sh
npm start
```

Abra http://127.0.0.1:4188. Para executar os testes:

```sh
npm test
```

Pode ser servido por qualquer servidor HTTP estático, incluindo GitHub Pages. Todos os caminhos são relativos para permitir hospedagem sob `/t-intervalos/`. Perfis e progresso ficam no navegador; limpar os dados do site remove esses dados locais. Áudio depende de uma interação do usuário.

## Fidelidade

Preserva as configurações das 30 fases, as modalidades e as regras de tempo/pontuação do original. Atingir a meta não encerra antecipadamente: a vitória é avaliada no fim do tempo. Erros consecutivos podem encerrar antes; erros contam após a pausa de feedback e acertos zeram a sequência.

O contexto menor usa a coleção de notas da armadura escolhida e sua tônica menor relativa quando fixada, como no código original. “Compostos” inclui também os intervalos simples. A classificação considera grafia diatônica, distinguindo, por exemplo, Dó–Ré♯ (segunda aumentada) de Dó–Mi♭ (terça menor).

A interface reutiliza fundos, logotipo e botões verdes originais, com adaptação responsiva. A pauta é SVG gerado na web e os sons das perguntas são sintetizados, com referência de afinação padrão; a posição/registro é adaptada às claves da versão web. Músicas e demonstrações instrumentais são os áudios recuperados do original. Não é uma exportação WebGL nem uma réplica pixel a pixel, e não recupera o projeto Unity.

Veja [o comportamento recuperado](docs/original-behavior.md) e [a validação](docs/validation.md).

## Créditos

Conceito e música: Glauber Santiago e Terence P. Santos. Programação original: Elias Ximenes. Arte: Emyr Ferrario. iMAX Games, MZO Interativa, UFSCar, UAB, SEaD e Licenciatura em Educação Musical.

Os recursos foram extraídos do pacote indicado pelo proprietário deste repositório. Os créditos foram mantidos; não se presumiu uma licença de terceiros ausente do pacote.
