# Central de acesso — ISAC MENU

Site estático em português, responsivo para celular e desktop. Cada uma das quatro etapas começa uma contagem regressiva de 10 segundos quando o link é aberto. Após a contagem, a pessoa confirma a etapa para liberar a seguinte. Ao final, a página mostra os dados de acesso e abre o download externo no MediaFire.

## Abrir localmente

Extraia o ZIP e abra `index.html` em um navegador. O site não precisa de servidor nem de dependências.

## Publicar com GitHub Pages

1. Crie ou abra um repositório no GitHub.
2. Envie `index.html` para a raiz do repositório.
3. No repositório, entre em **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**, escolha a branch principal e a pasta `/(root)`, e salve.
5. Aguarde o GitHub Pages publicar e abra o endereço mostrado nessa tela.

## Importante

A contagem e a liberação são feitas somente no navegador. Elas não verificam inscrição, like ou comentário e não protegem a chave: ela está no próprio código HTML e pode ser encontrada por quem inspecionar os arquivos. Para um controle de acesso real, seria necessário um backend com verificação apropriada.

O arquivo indicado permanece hospedado por terceiros. Este projeto não baixa, hospeda, analisa nem executa o arquivo. Confira a origem e examine o download com ferramentas de segurança antes de executá-lo.
