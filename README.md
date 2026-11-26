# Sobre mim

Site pessoal do Mateus Santos: livros e resenhas, gostos, hobbies e contato.

> **Versão alpha (v0.1).** O site ainda está mudando. Capas, resenhas e seções novas entram aos poucos, e o layout pode mudar entre uma visita e outra.

No ar: https://sobremim-three.vercel.app

Página estática em um único `index.html`, sem build e sem dependências.

## Editar conteúdo

Livros, resenhas, gostos e hobbies ficam no bloco `EDITE SEUS DADOS AQUI`, dentro do `<script>` no fim do `index.html`.

Livro: `["Título", "Autor", nota, "resenha", "capas/arquivo.webp"]` (resenha e capa são opcionais). Nota `null` mostra "Lendo agora".

Capas ficam em `capas/`, em 2:3 (600×900, .webp). Livro sem capa ganha uma capa gerada com título e autor.

## Deploy

Hospedado na Vercel. Cada push na branch `main` publica automaticamente. Os headers de segurança estão em `vercel.json`.

Direção visual: [DESIGN.md](DESIGN.md).
