# IBEN RH — Prévia do Sistema

Prévia interativa (HTML único, sem backend) do sistema de gestão de colaboradores da IBEN.

## Publicar no GitHub

1. Crie um repositório novo em https://github.com/new (ex.: `iben-rh-preview`).
2. Na sua máquina (ou pelo próprio site do GitHub, "Add file → Upload files"):
   ```bash
   git init
   git add index.html README.md
   git commit -m "Prévia do sistema IBEN RH"
   git branch -M main
   git remote add origin https://github.com/SEU_USUARIO/iben-rh-preview.git
   git push -u origin main
   ```
   Ou, mais simples: entre no repositório vazio no GitHub → **Add file → Upload files** → arraste o `index.html` → Commit.

## Publicar no Vercel

1. Acesse https://vercel.com/new
2. Clique em **Import Git Repository** e selecione o repositório que você acabou de criar (o Vercel pode pedir para conectar sua conta do GitHub na primeira vez).
3. Como é um HTML puro (sem framework), o Vercel detecta automaticamente como **Other/Static** — não precisa configurar build command nem output directory. Clique em **Deploy**.
4. Em ~30 segundos você recebe uma URL pública (ex.: `iben-rh-preview.vercel.app`).

Qualquer novo commit no branch `main` do GitHub gera um novo deploy automático no Vercel.

## Importante

Este arquivo é só uma **prévia visual interativa** — os dados ficam na memória do navegador de quem estiver acessando (cada pessoa que abrir vê a mesma base inicial, mas edições/exclusões feitas por uma pessoa não aparecem para outra, e tudo volta ao original se a página for recarregada). Não é o sistema real com banco de dados — esse está no outro pacote (`iben-rh.zip`) que já te enviei, com backend NestJS + PostgreSQL.

Login de teste:
- **dp@iben.eng.br** / `IBen@2026` (acesso total)
- **rh@iben.eng.br** / `IBen@123` (somente visualização)
