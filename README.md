# Sobre mim

Site pessoal do Mateus Santos: livros e resenhas, gostos, hobbies e contato.

> **Versão alpha (v0.1).** O site ainda está mudando. Capas, resenhas e seções novas entram aos poucos, e o layout pode mudar entre uma visita e outra.

No ar: https://sobremim-three.vercel.app

Página estática em um único `index.html`, sem build e sem dependências.

## Editar conteúdo

Livros, resenhas, gostos e hobbies ficam no bloco `EDITE SEUS DADOS AQUI`, dentro do `<script>` no fim do `index.html`.

Livro: `{titulo, autor, nota, ano, capa, resumo, resenha}`. Nota `null` mostra "Lendo agora"; `ano`, `capa` e `resenha` são opcionais. Clicar num livro abre a ficha com tudo isso.

A imagem de prévia do link é `og.png` (1200×630). A filosofia visual dela está em [arte/marginalia.md](arte/marginalia.md).

Capas ficam em `capas/`, em 2:3 (600×900, .webp). Livro sem capa ganha uma capa gerada com título e autor. Ao trocar uma capa por outra com o mesmo nome, aumente `CAPAS_V` no `index.html` para os navegadores baixarem a nova.

## Deploy

Hospedado na Vercel. Cada push na branch `main` publica automaticamente. Os headers de segurança estão em `vercel.json`.

Direção visual: [DESIGN.md](DESIGN.md).
