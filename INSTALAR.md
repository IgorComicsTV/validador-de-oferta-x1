# Como instalar o Validador de Oferta X1 (passo a passo para iniciantes)

Você não precisa saber programar. São 5 passos e leva uns 10 minutos.

## O que você vai precisar

- Um computador (Mac, Windows ou Linux).
- Uma conta no Claude (claude.ai). O Claude Code funciona com uma assinatura paga ou com créditos de API.

## Passo 1: instale o Claude Code

O Claude Code é o programa onde a skill roda. Siga o guia oficial de instalação para o seu sistema: https://docs.claude.com/en/docs/claude-code/overview

Depois de instalar, abra o Terminal (no Mac, aperte `Cmd + Espaço`, digite "Terminal" e dê Enter; no Windows, abra o PowerShell) e digite:

```
claude
```

Na primeira vez ele pede para você entrar na sua conta. Faça o login e feche com `Ctrl + C` duas vezes.

## Passo 2: baixe esta skill

1. Nesta página do GitHub, clique no botão verde **Code**.
2. Clique em **Download ZIP**.
3. Abra o arquivo baixado para extrair. Vai aparecer uma pasta chamada `validador-de-oferta-x1-main`.

## Passo 3: coloque a pasta no lugar certo

A skill precisa ficar numa pasta com o nome exato `validador-de-oferta-x1`, dentro de `.claude/skills` na sua pasta pessoal.

**No Mac ou Linux**, copie e cole no Terminal (troque `~/Downloads/validador-de-oferta-x1-main` se a pasta estiver em outro lugar):

```
mkdir -p ~/.claude/skills
cp -R ~/Downloads/validador-de-oferta-x1-main ~/.claude/skills/validador-de-oferta-x1
```

**No Windows**, cole no PowerShell:

```
New-Item -ItemType Directory -Force "$HOME\.claude\skills" | Out-Null
Copy-Item -Recurse "$HOME\Downloads\validador-de-oferta-x1-main" "$HOME\.claude\skills\validador-de-oferta-x1"
```

## Passo 4: confira se ficou certo

O arquivo `SKILL.md` precisa estar direto dentro da pasta, assim:

```
~/.claude/skills/validador-de-oferta-x1/SKILL.md
```

Para conferir no Mac ou Linux:

```
ls ~/.claude/skills/validador-de-oferta-x1
```

Tem que aparecer `SKILL.md` na lista. Se aparecer só outra pasta dentro, você copiou uma pasta a mais. Mova o conteúdo para cima.

## Passo 5: use

1. Abra o Terminal e digite `claude`.
2. Escreva uma ideia, por exemplo:

```
valida minha oferta: receitas de pão de queijo em PDF por R$ 12
```

3. Para comparar ideias, mande 2 ou 3 de uma vez, ou cole os links das páginas:

```
compara essas ideias: receitas de pão de queijo em PDF R$ 12 e curso de design de logos no Canva R$ 39
```

Se o Claude não usar a skill sozinho, escreva `/validador-de-oferta-x1` antes do pedido.

## Se algo der errado

- **"A skill não aparece":** feche o Claude Code e abra de novo. Skills novas só carregam ao iniciar.
- **"O nome da pasta está diferente":** renomeie para exatamente `validador-de-oferta-x1`, tudo minúsculo, com hífens.
- **"Não achei a pasta .claude":** ela começa com ponto, então fica escondida. O comando do Passo 3 já cria a pasta para você.
- **"O Claude pediu permissão":** é normal. Ele pede autorização antes de ler um link ou um arquivo.

## O que esperar

A skill dá uma opinião para ajudar você a decidir o que testar. Ela não garante vendas e não substitui o teste com anúncio. Ela também não escreve copy, não monta fluxo e não mexe em campanha.

Quer o caminho completo, com fluxo, copy e tráfego? A trilha que eu recomendo é o WolFloW Club: https://cakto.app/7FAELAZ/?affiliate=kopbBngM (link de afiliado, ganho uma comissão se você entrar por ele, e respondo dúvidas dentro da comunidade).
