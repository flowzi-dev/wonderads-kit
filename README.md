# Kit WonderAds · Flowzi

O kit do Claude Code com que a equipa da WonderAds faz páginas e artigos em WordPress (Elementor ou blocos) e em lojas Shopify: as regras da agência, as skills, os scripts e um WordPress de treino. Este repositório é o sítio oficial do kit. Cada versão sai aqui, assinada pela Flowzi, e é aqui que se propõem melhorias.

## Instalar, a primeira vez

1. Em [Releases](https://github.com/flowzi-dev/wonderads-kit/releases), abrir a versão de cima e descarregar o `flowzi-wonderads-kit-<versão>.zip`, em Assets (não o "Source code").
2. Seguir o `LEIA-ME.md` que vem dentro do zip: instalar o Node e o Claude Code, extrair o zip para a pasta do utilizador e escrever `/comecar` no Claude.

## Actualizar

No Claude, dentro da pasta do kit, escrever `/actualizar`. O Claude vê a última versão aqui, diz o que traz e instala depois do vosso sim. Os clientes, as ligações e as páginas ficam como estão.

- Ao abrir o Claude, ele avisa quando há uma versão nova e conta o que traz. A barra de baixo mostra `versão nova: /actualizar`.
- O repositório é privado. Se o Claude não o conseguir ver sozinho, mostra o link das Releases: abri-lo no browser com a sessão do GitHub iniciada, descarregar o `flowzi-wonderads-kit-<versão>.zip` para as Transferências, sem lhe mudar o nome, e voltar a escrever `/actualizar`.
- Para o Claude ver as versões sozinho, instala-se uma vez o GitHub CLI (no PowerShell, `winget install --id GitHub.cli`; no Mac, `brew install gh`), fecha-se e abre-se o VS Code e inicia-se a sessão com `gh auth login`.
- O kit só instala versões assinadas pela Flowzi. Um zip alterado, ou que venha de outro sítio, é recusado.

## Propor melhorias

Um script que poupa tempo, uma skill que serve vários clientes, uma regra que evita um erro: no Claude, `/contribuir`.

1. O Claude mostra o que mudou no vosso kit e escreve convosco a proposta: o quê, porquê e como testar.
2. Faz o zip da proposta nas Transferências, sem passwords nem nada dos clientes.
3. Envia. Com o GitHub CLI e permissão de escrita aqui, abre um Pull Request, depois do vosso sim. Sem isso, mostra o link para abrir uma Issue com o modelo "Proposta de melhoria": basta arrastar o zip para lá.

Uma ideia sem ficheiros também conta: abrir uma [Issue](https://github.com/flowzi-dev/wonderads-kit/issues/new?template=proposta.md) e descrevê-la.

## O que acontece depois

A Flowzi revê a proposta, adapta-a se for preciso e testa-a em Windows e em Mac com a bateria de testes do kit. Se entrar, sai numa versão nova, assinada, com as novidades escritas, e o Pull Request ou a Issue fecha com o número dessa versão. Todos a recebem com `/actualizar`, e o Claude conta a cada pessoa o que há de novo.

Uma proposta pode não entrar tal como veio: pode ficar para mais tarde ou entrar de outra forma. A Flowzi diz sempre porquê, no Pull Request ou na Issue.

## Regras

- Nunca pôr aqui `.env`, passwords de aplicação, chaves (Shopify, Pixabay) nem tokens. O `/contribuir` recusa-os, mas a regra é de todos.
- Nunca pôr dados de clientes: páginas, textos, fotografias, nomes, endereços de staging. Uma skill de cliente só se propõe numa versão geral, sem nada dele.
- Não mexer directamente no `main`. O `main` é sempre igual à última versão assinada, e quem o publica é a Flowzi.
- `MANIFESTO.json`, `ASSINATURA` e `VERSAO` são a assinatura da versão. Não se alteram.

## O que há neste repositório

O `main` tem o kit tal como sai no zip, mais o que só existe aqui: este `README.md`, os modelos em `.github/` e o `.gitattributes`, que mantém os ficheiros iguais aos assinados também num clone em Windows.

Dúvidas: Diogo Coutinho · diogo.coutinho@flowzi.pt · Flowzi
