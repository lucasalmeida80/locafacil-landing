# LocaFácil — Landing Page

Página de divulgação do **LocaFácil**, o app que organiza tudo que você aluga
(imóveis, veículos e equipamentos): contratos, cobranças, comprovantes, chamados
e relatórios.

Site **estático** de um arquivo só (`index.html`), com **Tailwind via CDN** e
fonte **Nunito**. Sem build, sem dependências.

## Rodar localmente

```bash
npx serve -l 8090 .
# abre em http://localhost:8090
```

## Deploy (Vercel / Netlify / GitHub Pages)

É um site estático — qualquer host serve. No Vercel/Netlify basta conectar este
repositório (sem comando de build, _output dir_ = raiz) ou arrastar a pasta.

## Configurar o botão "Entrar"

No fim do `index.html` há:

```js
const APP_URL = '#';
```

Troque `'#'` pela URL do app web (export do Expo), ex.: `https://app.locafacil.com.br`.
Aí todos os botões "Entrar / Começar grátis" passam a abrir as funções do app.
