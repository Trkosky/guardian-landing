# Guardian Gestão Segura de Risco — Landing Page

Landing page institucional da **Guardian Gestão Segura de Risco Ltda.**, empresa de cadastros, consultas e análise de perfil de risco para o setor de transporte de cargas.

Site estático (HTML + CSS + JS puro, sem build/dependências) pronto para publicar no GitHub Pages.

## Estrutura

```
gardian-landing/
├── index.html          # página principal
├── css/style.css        # estilos (paleta, tipografia, responsividade)
├── js/script.js         # menu mobile, dropdown, botão voltar ao topo, newsletter
└── assets/
    └── shield-icon.svg  # logo/ícone da marca (também usado como favicon)
```

## Rodar localmente

Qualquer servidor estático funciona. Exemplo:

```bash
npx serve .
# ou
python -m http.server 8080
```

Depois acesse `http://localhost:8080`.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (ex: `guardian-landing`) e envie estes arquivos:
   ```bash
   git init
   git add .
   git commit -m "Landing page Guardian Gestão Segura de Risco"
   git branch -M main
   git remote add origin https://github.com/SEU_USUARIO/gardian-landing.git
   git push -u origin main
   ```
2. No GitHub: **Settings → Pages → Source** selecione a branch `main` e a pasta `/ (root)`.
3. O site ficará disponível em `https://SEU_USUARIO.github.io/gardian-landing/`.

### Domínio próprio (www.gauardingestaosegura.com.br)

Para usar o domínio próprio em vez do endereço `github.io`:

1. No provedor de DNS do domínio, crie um registro **CNAME** apontando `www` para `SEU_USUARIO.github.io`.
2. Crie um arquivo `CNAME` (sem extensão) na raiz do projeto contendo apenas:
   ```
   www.gauardingestaosegura.com.br
   ```
3. Em **Settings → Pages → Custom domain**, informe o mesmo domínio e aguarde a verificação/HTTPS do GitHub.

## Identidade visual

| Cor | Hex |
|---|---|
| Laranja (primária) | `#F58220` |
| Preto/Grafite | `#1D1D1D` |
| Cinza | `#6B6B6B` |
| Branco | `#FFFFFF` |

Tipografia: **Montserrat** (Google Fonts).
