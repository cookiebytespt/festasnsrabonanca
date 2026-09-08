# Festas em Honra de Nossa Senhora da Bonança 2026

Site estático das festas de Vila Praia de Âncora (9–13 de setembro de 2026), alojado no GitHub Pages em **https://festasnsrabonanca.com**.

## Estrutura

- `index.html` — página única em português (programa, comissão, merchandising). HTML, CSS e JS inline, sem dependências além das fontes Google.
- `en/index.html` e `fr/index.html` — versões inglesa e francesa da mesma página (assets partilhados em `../assets/`). O seletor de idioma (PT/EN/FR) está no cabeçalho.
- `assets/` — cartaz, programa em imagem, retratos da comissão e merchandising (otimizados a partir dos posts do Instagram).
- `assets/apoios/{gold,silver,bronze}/` — anúncios dos patrocinadores (recortados do programa impresso). Os contactos de cada patrocinador (site, telefone, Instagram, Facebook, e-mail) estão nos ícones por baixo de cada anúncio.
- `CNAME` — domínio personalizado para o GitHub Pages.
- `.nojekyll` — desativa o processamento Jekyll.

## Publicar

1. Criar um repositório no GitHub e enviar o conteúdo desta pasta para o ramo `main`.
2. Em *Settings → Pages*, escolher *Deploy from a branch* → `main` / `/ (root)`.
3. No DNS de `festasnsrabonanca.com`, apontar:
   - registos `A` para `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` de `www` para `<utilizador>.github.io`
4. Em *Settings → Pages*, confirmar o domínio e ativar *Enforce HTTPS*.

## Editar o programa

O programa está diretamente no `index.html` (e em `en/index.html` / `fr/index.html` para as versões inglesa e francesa) (uma `<section class="panel">` por dia, com `<li class="ev">` por evento). Basta editar o texto e fazer commit.

---
Site desenvolvido por [CookieBytes](https://cookiebytes.pt).
