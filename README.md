# Organização Financeira — V2

Versão preparada para GitHub Pages + Appwrite TablesDB.

## O que foi corrigido
- Login e cadastro reais com Appwrite Authentication.
- Recuperação de senha por e-mail.
- Sessão persistente no navegador.
- Uso do Appwrite `TablesDB` para as tabelas existentes.
- Dados vinculados ao usuário autenticado.
- PWA com manifest válido e ícones 192x192 e 512x512.
- Service Worker com atualização de cache (`v2`) para evitar que o celular fique preso na versão antiga.
- Botão de instalação do aplicativo quando o navegador disponibiliza a instalação.

## Appwrite configurado
Endpoint: `https://nyc.cloud.appwrite.io/v1`
Projeto: `6b01e299000b19ac36ce`
Database: `6b01e350001ca47807e5`

## Importante no Appwrite
As tabelas precisam permitir CREATE no nível da tabela. Com Row Security ativado, as linhas criadas pelo Client SDK recebem permissões do criador conforme a política do Appwrite.

O domínio `mihcatherine.github.io` precisa continuar cadastrado como Web Platform no projeto Appwrite, porque o domínio publicado faz as chamadas do navegador para o Appwrite.

## Publicação
Suba o conteúdo desta pasta para o repositório do GitHub Pages, mantendo `index.html` na raiz.

Depois da publicação, abra o endereço pelo Chrome/Edge no Android. Para instalar, use o botão que aparece no Início quando o navegador disponibilizar a instalação; caso não apareça, use o menu ⋮ do navegador > `Instalar aplicativo` ou `Adicionar à tela inicial`.

O ZIP não é um APK. O APK exigiria empacotar este projeto em Android. Esta versão é um PWA instalável.
