# Atividades — app de jogos para 4 a 5 anos

App web com 5 jogos (ligar os pontos, sudoku de frutas, qual vem depois?, contar e primeiras letras). Tudo em português, sem anúncios, sem coleta de dados, funciona offline depois de aberto uma vez.

## O jeito mais simples (iPhone / iPad)

Você só precisa do arquivo **`index.html`**.

1. Crie um repositório no GitHub (ex.: `atividades`).
2. Envie o `index.html` para o repositório (botão **Add file › Upload files**).
3. Abra **Settings › Pages**, em **Branch** escolha `main` e pasta `/root`, salve.
4. Aguarde ~1 minuto. O GitHub mostra o endereço, algo como
   `https://SEU-USUARIO.github.io/atividades/`.
5. Abra esse endereço no **Safari** do iPhone/iPad, toque em **Compartilhar › Adicionar à Tela de Início**.

Pronto: vira um ícone na tela inicial, abre em tela cheia e funciona sem internet.

## Versão completa (recomendada: offline garantido + instalável no Android)

Para a instalação funcionar melhor — ícone próprio, cache offline confiável e o botão "Instalar" no Android/Chrome — envie **todos os arquivos desta pasta** para o repositório, mantendo os nomes:

```
index.html
manifest.webmanifest
sw.js
icon-192.png
icon-512.png
```

O resto do passo a passo (Pages) é igual. No Android/Chrome aparece a opção **Instalar app**; no iPhone/iPad, **Adicionar à Tela de Início**.

## Observações

- Precisa estar em **HTTPS** para instalar como app — o GitHub Pages já serve em HTTPS, então está coberto.
- Se você atualizar os arquivos, troque a linha `const CACHE = "atividades-v1"` no `sw.js` para `"atividades-v2"` (e assim por diante) para forçar a atualização nos aparelhos que já instalaram.
- O progresso (jogos concluídos, som ligado/desligado) fica salvo só no próprio aparelho.
