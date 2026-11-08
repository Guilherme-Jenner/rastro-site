# rastro-site

Páginas estáticas do Rastro, publicadas pelo GitHub Pages. Cada tela é um arquivo HTML:

| Arquivo | Conteúdo |
|---|---|
| `index.html` | Página inicial (o que o app faz e não faz) |
| `privacidade.html` | Política de Privacidade (URL exigida pela App Store e pela Play Store) |
| `termos.html` | Termos de Uso |
| `suporte.html` | Suporte e perguntas frequentes (URL de suporte da App Store) |
| `en/` | Versão em inglês (`index`, `privacy`, `terms`, `support`), tradução dos textos em português |
| `style.css` | Estilo comum (cores do design system do app, com modo escuro) |

Sem build: é só HTML e CSS. `.nojekyll` desliga o Jekyll do Pages. Sem fontes nem scripts externos, para o site não fazer requisição a terceiros.

## Manutenção dos textos

- Os textos descrevem o app **como ele é hoje**: sem conta e sem servidor próprio, dados só no aparelho, reconhecimento de fala no aparelho, iCloud opcional. **Se isso mudar no app, atualize a política antes de publicar a versão**, e confira a ficha "Privacidade do app" na App Store Connect.
- Pontos que a política afirma e que o app precisa continuar cumprindo: nenhum SDK de análise ou publicidade; áudio não é gravado; imagem de compartilhamento sem citações do diário; sem conta e sem coleta de dados de ninguém (a seção "Crianças e adolescentes" depende disso). Mantenha a classificação etária da App Store coerente com esse texto.
- **Ao mudar um texto em português, mude também o equivalente em `en/`** (o português é o original).
- **Ainda sem revisão jurídica.**

## Publicar

Settings → Pages → Deploy from a branch → `main` / `(root)`.

URLs usadas nas lojas (ajuste ao usuário/repositório reais):

- Política de Privacidade: `https://<usuario>.github.io/<repositorio>/privacidade.html`
- Suporte: `https://<usuario>.github.io/<repositorio>/suporte.html`
- Em inglês: `.../en/privacy.html` e `.../en/support.html`
