---
tipo: readme
data: 2026-07-30
produzido-por: Raphael Sousa Pizani Silva (OAB/BA 32.472)
versao-core: 1.0
---

# Verificar lendo a fonte

> Skill para assistentes de IA, em uma linha: **índice localiza, fonte autoriza**.

Nenhuma afirmação sobre o estado do mundo — o que existe, o que foi juntado, o
que diz o documento — se faz a partir de representação. Faz-se abrindo a coisa.

É a menor da família e a que mais muda o comportamento no dia a dia.

## Calibrada por consequência, não uniforme

O esforço de abrir uma fonte é quase constante. O custo de errar, não: errar a
data de um prazo não se compara a errar o nome de um município na qualificação.
Verificação uniforme para tudo é regra impossível — e regra impossível não é
seguida com moderação, é ignorada por inteiro, inclusive onde importava.

**Fonte primária obrigatória**, sem exceção: o que entra em peça ou documento que
sai do escritório; o que se afirma a cliente, juízo ou terceiro; o que embasa
decisão difícil de reverter; e **data e termo inicial de prazo, sempre** — a
categoria de erro mais cara.

**Representação tolerada** em triagem, hipótese de trabalho e planejamento
interno, sob duas condições: rotule como não verificado ("segundo o índice", "a
conferir"), e verifique **no momento em que a hipótese for promovida a
afirmação**. A promoção é o gatilho.

## O que conta como representação

Índice, ficha, resumo, planilha de controle, handoff, a memória persistente do
assistente, **o que foi dito antes na própria conversa**, a sua lembrança — e
**"fulano disse que conferiu"**, a verificação delegada.

Os dois últimos são os mais perigosos. A lembrança não parece uma fonte: parece
conhecimento. E a verificação delegada tem a forma de verificação, mas o que
chega até você é o relato dela. Delegar é legítimo; perder o rastro não é. Quem
verificou informa **o que abriu e o que viu** — "abri o Num. 4455, pág. 2, a
procuração está assinada em 12/03" vale; "conferi, está tudo certo" não vale.

## Antes de afirmar que NÃO existe — com critério de parada

O erro mais caro é declarar ausência depois de uma busca só. **"Procurei e não
achei" não é "não existe"**: é "minha busca falhou", e as duas frases levam a
decisões opostas — pedir ao cliente documento que ele já mandou, refazer pesquisa
feita, comprar consulta paga desnecessária.

Cinco frentes: varrer o acervo inteiro (não só a pasta óbvia); variar o termo de
busca; buscar por conteúdo, não só por nome de arquivo (o nome mente; o texto
dentro, não — e documento em imagem não aparece em busca textual); checar os
canais de entrada; e **ler o resultado** — busca lançada e não lida não foi
feita.

**E então parar.** A busca termina quando cada frente foi percorrida uma vez, com
termos variados. Não se repete frente já coberta esperando resultado diferente.
Se o prazo aperta antes de fechar as cinco, para-se e declara-se a cobertura
parcial: ausência parcial declarada vale mais que ausência total inventada.

## Quando a fonte primária está inacessível

O sistema do tribunal fora do ar na véspera, o cartório que só abre segunda.
"Não afirme" não resolve — o advogado precisa protocolar. Classifique a
indisponibilidade; **registre a tentativa** com data, hora e captura (sem
registro, não se fundamenta prorrogação); afirme pela melhor representação
disponível **nomeando-a** ("segundo cópia dos autos obtida em DD/MM, estando o
sistema indisponível"); e ancore a redação no que se pôde ver.

O que descredencia não é a fonte secundária — é apresentá-la como se fosse a
primária. **Não se perde prazo por pureza de método.**

## As três frases proibidas

"Deve estar em..." · "Pelo que me lembro..." · "Provavelmente já foi feito".

Todas podem ser ditas, desde que seguidas de "vou confirmar" — e seguidas mesmo.

## Instalação

```bash
git clone https://github.com/pizaniadv/verificar-lendo-a-fonte.git \
  ~/.claude/skills/verificar-lendo-a-fonte
```

Skills seguem o padrão aberto [Agent Skills](https://agentskills.io).

## Como usar

`/verificar-lendo-a-fonte`, ou: "confere se" · "isso existe mesmo" · "cadê o
documento" · "já temos isso" · "tem certeza?" · "sistema fora do ar".

## Executa sozinha

Não depende de outra skill.
[`antialucinacao-juridica`](https://github.com/pizaniadv/antialucinacao-juridica)
aplica esta disciplina em duas camadas;
[`handoff-de-sessao`](https://github.com/pizaniadv/handoff-de-sessao) produz
representação para a próxima sessão — e esta skill é a razão pela qual quem
recebe reconfere.

## Licença

Licenciamento duplo, ambos copyleft, ambos com **atribuição nominal
obrigatória**: **[AGPL-3.0](LICENSE)** e **[CC BY-SA 4.0](LICENSE-DOCS)**. Uso
próprio não gera obrigação; distribuir ou servir a terceiros exige abrir o
código e manter a atribuição. O [NOTICE](NOTICE) é parte da licença.

## Autor

**Raphael Sousa Pizani Silva** — OAB/BA 32.472
[github.com/pizaniadv](https://github.com/pizaniadv)

Histórico de versões no [CHANGELOG](CHANGELOG.md).
