# CLAUDE.md — TESTEDOS100DIAS

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** TESTEDOS100DIAS
**Nicho:** Automotivo
**Keywords:** O Teste dos 100 dias e uma avaliacao de longa duracao que
**Paleta de cores:** gold | **Fonte:** montserrat

O Teste dos 100 dias é uma avaliação de longa duração que estreou com pioneirismo na internet em julho de 2007. Nesse período, já realizamos avaliações com modelos diferentes de carros e motocicletas que foram submetidos a testes rigorosos na pista, medições de consumo e avaliações de inúmeros jornalistas e colaboradores da Motorpress Brasil Editora. Participe com seus comentários, críticas e sugestões e nos ajude a fazer um teste sempre mais perto do que busca o consumidor. Equipes revista Carro e Motociclismo.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-C |
| Hero | Hero-C |
| Features | Features-C |
| About Section | About-A |
| Posts | Posts-J |
| Footer | Footer-H |
| Página Sobre | Sobre-A |
| Página Contato | Contato-C |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
