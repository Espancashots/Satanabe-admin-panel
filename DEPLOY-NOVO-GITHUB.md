# Publicar esta cópia do Satanabe Admin em outro GitHub

Esta cópia mantém a MESMA Supabase e, portanto, administra as mesmas keys, clientes, revendedores, patches, logs e configurações já usados pelo Satanabe External.

## Passos
1. Crie um repositório novo na nova conta do GitHub.
2. Extraia este ZIP.
3. Envie TODOS os arquivos da raiz para a raiz do repositório (index.html, app.js, styles.css etc.).
4. No GitHub: Settings > Pages.
5. Em Build and deployment, escolha Deploy from a branch.
6. Branch: main; pasta: / (root).
7. Salve e abra a URL fornecida pelo GitHub Pages.

## O que foi preservado
- Supabase: https://agkjutuvfjcahckhjkra.supabase.co
- Mesmas Edge Functions do Admin.
- Mesmo bucket `patches-3105`.
- Mesmo sistema de login/allowlist.
- Mesmo Satanabe External e dados já cadastrados.
- Mesmo painel de revendedor externo já configurado.

## Nova organização de patches
O formulário de importar/editar patch agora oferece as abas:
- RANKEADA
- APOSTADO
- SKINS

O frontend envia esse valor como `interfaceTab` para `admin-patches-api`, sem trocar a Supabase.

## Atenção
Não coloque `service_role` no repositório. O `app.js` contém apenas a chave publicável do projeto, como na versão original.
