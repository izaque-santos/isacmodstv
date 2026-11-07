# Central de acesso — ISAC MENU

Site estático em português, responsivo para celular e desktop. Cada uma das quatro etapas começa uma contagem regressiva de 10 segundos quando o link é aberto. Após a contagem, a pessoa confirma a etapa para liberar a seguinte. Ao final, a página mostra os dados de acesso e abre o download externo no MediaFire.

## Publicar no GitHub pelo Termux

O pacote inclui `publicar-termux.sh`, que extrai `index.html` e `README.md` do ZIP e os envia para `izaque-santos/isacmodstv`. O script verifica se o repositório continua vazio, pede confirmação antes do envio e não sobrescreve um repositório que já tenha commits. A página contém a chave `VDASQUTH`; o próprio script avisa que ela ficará pública e só prossegue se você digitar `SIM`.

1. Instale o Termux por uma fonte oficial e abra o aplicativo.
2. No Termux, execute `termux-setup-storage` e permita o acesso aos arquivos.
3. Baixe este ZIP para a pasta Downloads do Android e extraia-o.
4. No Termux, instale o necessário: `pkg update -y && pkg install -y git unzip gh`.
5. Entre na pasta extraída. Um exemplo, se ela estiver em Downloads: `cd ~/storage/downloads/site-isac-acesso`.
6. Execute: `bash publicar-termux.sh ~/storage/downloads/site-isac-acesso.zip`.
7. Se solicitado, autorize o GitHub no navegador. Confira o aviso do script e digite `SIM` para enviar.

Se o ZIP estiver em outro local, passe o caminho correto como argumento. A conta GitHub autenticada precisa ter permissão para enviar arquivos ao repositório indicado.

## Ativar o GitHub Pages

Depois que o envio terminar, abra o repositório `izaque-santos/isacmodstv` no GitHub. Vá em **Settings → Pages** e, em **Build and deployment**, selecione **Deploy from a branch**, escolha `main` e `/(root)`, e salve. O endereço do site aparecerá nessa tela após a publicação.

## Abrir localmente

Extraia o ZIP e abra `index.html` em um navegador. O site não precisa de servidor nem de dependências.

## Importante

A contagem e a liberação são feitas somente no navegador. Elas não verificam inscrição, like ou comentário e não protegem a chave: ela está no próprio código HTML e pode ser encontrada por quem inspecionar os arquivos. Para um controle de acesso real, seria necessário um backend com verificação apropriada.

O arquivo indicado permanece hospedado por terceiros. Este projeto não baixa, hospeda, analisa nem executa o arquivo. Confira a origem e examine o download com ferramentas de segurança antes de executá-lo.
