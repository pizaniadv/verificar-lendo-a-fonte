---
tipo: readme
data: 2026-07-30
produzido-por: Raphael Sousa Pizani Silva (OAB/BA 32.472)
versao-core: 1.0
---

# Verificar lendo a fonte

> Skill para assistentes de IA, em uma linha: **índice localiza, fonte
> autoriza**.

Nenhuma afirmação sobre o estado do mundo — o que existe, o que foi juntado, o
que diz o documento — se faz a partir de representação. Faz-se abrindo a coisa.

É a menor das skills desta família e a que mais muda o comportamento no dia a
dia.

## O que conta como representação (e portanto não prova)

Índice de pasta · ficha interna · resumo · planilha de controle · handoff da
sessão anterior · a memória persistente do assistente · **o que foi dito antes
nesta mesma conversa** · a sua própria lembrança.

O último é o mais perigoso, porque não parece uma fonte: parece conhecimento.

Representação e realidade divergem por três motivos banais: **defasagem** (o
índice foi escrito quando a pasta tinha outra coisa), **otimismo** (registrou-se
a intenção de juntar o documento, e a intenção sobreviveu ao fato de nunca ter
juntado) e **herança** (o resumo copiou de outro resumo, e o erro original está
a quatro saltos).

## O que ela faz

- **Antes de afirmar que existe:** confere quatro coisas — existe, é o que diz
  ser, está legível e completo, está vigente.
- **Antes de afirmar que NÃO existe:** aplica o protocolo de busca exaustiva.
  "Procurei e não achei" é *"minha busca falhou"*, não *"não existe"* — e as
  duas frases levam a decisões opostas: pedir ao cliente documento que ele já
  mandou, refazer pesquisa pronta, comprar consulta paga à toa. Inclui a regra
  de que **busca lançada e não lida não foi feita**.
- **Antes de pedir ao cliente:** procura no acervo e **nos autos** — procuração
  e contrato social costumam já estar juntados por você mesmo.
- **Antes de dizer "não é possível":** verifica se varreu os caminhos, porque
  declarar impossibilidade por desconhecimento é alucinação por omissão.
- **Ensina a declarar a verificação**: "confirmado, Num. 4455 - Pág. 2,
  conferido agora" · "não localizei; procurei em A, B, C, com os termos D e E".

## As três frases proibidas

"Deve estar em..." · "Pelo que me lembro..." · "Provavelmente já foi feito".

Todas podem ser ditas, desde que seguidas de "vou confirmar" — e seguidas
mesmo.

## Instalação

```bash
git clone https://github.com/pizaniadv/verificar-lendo-a-fonte.git \
  ~/.claude/skills/verificar-lendo-a-fonte
```

Skills seguem o padrão aberto [Agent Skills](https://agentskills.io).

## Como usar

`/verificar-lendo-a-fonte`, ou: "confere se", "isso existe mesmo", "cadê o
documento", "já temos isso", "tem certeza?".

## A família

- [`antialucinacao-juridica`](https://github.com/pizaniadv/antialucinacao-juridica)
  — aplica esta disciplina em duas camadas: o fato contra o documento, a fonte
  contra a fonte primária.
- [`handoff-de-sessao`](https://github.com/pizaniadv/handoff-de-sessao) —
  produz representação para a próxima sessão; esta skill é a razão pela qual
  quem recebe reconfere.

## Licença

Licenciamento duplo, ambos copyleft, ambos com **atribuição nominal
obrigatória**: **[AGPL-3.0](LICENSE)** para o componente executável e
**[CC BY-SA 4.0](LICENSE-DOCS)** para a obra textual.

Uso no seu escritório não gera obrigação nenhuma. **Distribuir** versão
modificada, ou **oferecê-la a terceiros como serviço**, exige abrir o código e
manter a atribuição. O [NOTICE](NOTICE) é parte da licença.

## Autor

**Raphael Sousa Pizani Silva** — OAB/BA 32.472
[github.com/pizaniadv](https://github.com/pizaniadv)
