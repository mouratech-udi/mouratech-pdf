# Mouratech PDF

Guia da versão 1.7.0 para Windows de 64 bits.

O Mouratech PDF permite ler, anotar, organizar, imprimir e assinar PDFs no seu computador. Você só precisa de certificado digital para assinar com um A1.

## Instalar e abrir um PDF

1. Execute o instalador **Mouratech-PDF-1.7.0-x64.msi** recebido com esta versão. As versões públicas ficam na [página de downloads](https://github.com/mouratech-udi/mouratech-pdf/releases).
2. Execute o instalador na conta do Windows em que usará o aplicativo.
3. Abra **Mouratech PDF** pelo menu **Iniciar**. Clique em **Abrir** e escolha um documento.

Você também pode clicar com o botão direito em um PDF no Explorador de Arquivos e escolher **Abrir com → Mouratech PDF**. Para atualizar uma instalação feita pelo MSI, execute o instalador da versão mais recente.

## Ler, buscar e imprimir

| Para | Faça assim |
| --- | --- |
| Mudar de página | Clique em uma miniatura à esquerda ou use as setas no rodapé, onde aparecem a página atual e o total. |
| Ajustar o zoom | Gire a roda do mouse sobre o documento. Clique em **Ajustar página** para ver a folha inteira. |
| Rolar a página | Segure o botão esquerdo e arraste a folha ou use as barras de rolagem. |
| Buscar uma palavra | Pressione **Ctrl+F**, digite o termo e pressione **Enter**. **Enter** avança, **Shift+Enter** volta e **Esc** fecha a busca. Em documentos digitalizados, a busca depende de uma camada de texto pesquisável. |
| Imprimir | Pressione **Ctrl+P** ou clique em **Imprimir**. Escolha a impressora e o intervalo de páginas. |

## Gerar PDFs pela impressora Mouratech PDF

Abra **Ferramentas → Configurar impressora virtual PDF** e escolha uma pasta de entrada. O aplicativo cria a impressora **Mouratech PDF** usando o componente Microsoft Print to PDF instalado no Windows.

1. Mantenha a janela principal do Mouratech aberta ou minimizada.
2. No programa de exames, escolha **Imprimir → Mouratech PDF**.
3. Na janela do Windows, salve o PDF na pasta de entrada escolhida.
4. Aguarde alguns segundos. O documento será aberto em uma nova janela do Mouratech para conferência e assinatura.
5. Use **Assinar digitalmente** ou **Assinar e imprimir**, conforme desejar.

**Ferramentas → Abrir pasta de entrada PDF** mostra a pasta configurada. Os arquivos presentes antes de abrir o leitor ficam disponíveis nessa pasta. A abertura automática acompanha arquivos novos e novas gravações enquanto a janela principal está aberta. Cópias com o sufixo **_assinado.pdf** ficam fora dessa abertura automática.

Se o programa de exames utiliza a impressora padrão escolhida ao iniciar, selecione Mouratech PDF como padrão nas configurações do Windows antes de abrir o programa de exames. A impressora física preferida é escolhida separadamente no Mouratech.

## Salvar a impressora física preferida

Abra **Ferramentas → Configurar impressora física**, selecione a impressora da clínica, o papel, a orientação e a quantidade de cópias. Clique em **Salvar preferência**. A configuração fica salva para a sua conta do Windows e é usada nas próximas aberturas do Mouratech.

**Imprimir** abre a janela de impressão com essa preferência selecionada, permitindo ajustar as opções para aquele documento. **Assinar e imprimir** usa a preferência salva para enviar a cópia assinada diretamente à impressora depois de salvar e conferir a assinatura. Se a impressora ou o papel salvo estiver indisponível, o aplicativo pede uma nova seleção.

**Assinar digitalmente** continua disponível como opção independente para assinar e salvar o PDF. Use **Assinar e imprimir** quando também quiser uma cópia em papel. O gerador de PDF pode continuar definido como impressora padrão do Windows para o programa de exames.

## Assinar digitalmente com um certificado A1

1. Abra o PDF e clique em **Assinar digitalmente**.
2. Selecione seu certificado. Confira o titular e a data de vencimento.
3. Em **Página para assinar**, escolha a página desejada. O padrão é a terceira página, ou a última disponível em documentos menores. Na prévia, clique logo abaixo de onde deseja colocar o carimbo. Ele aparece **acima do ponto escolhido**. Se a posição estiver bloqueada, escolha uma área branca livre de texto, linhas e imagens.
4. Marque **Confirmo que desejo assinar este documento** e clique em **Assinar e salvar cópia**.
5. Escolha a pasta e o nome da cópia. Para `contrato.pdf`, por exemplo, o nome sugerido é `contrato_assinado.pdf`. Se o destino já existir, escolha outro nome. O original é preservado.

O carimbo mostra o titular, a autoridade emissora e a data e hora do computador com o fuso. Quando o certificado traz uma imagem compatível do emissor, ela aparece ao lado do texto. A hora registrada vem do computador e não tem certificação independente de uma autoridade de tempo.

**Para assinar vários PDFs**, salve as alterações antes de começar. Clique em **Assinar lote**, selecione os arquivos e revise cada documento. Clique em **Aprovar para o lote** ou **Pular este arquivo**. O primeiro certificado aprovado será usado em todo o lote. Após a confirmação final, cada cópia é salva na pasta do original com o sufixo `_assinado.pdf`. A janela final mostra o resultado de cada arquivo.

**Para inserir uma assinatura manuscrita como imagem**, escolha **Assinar por imagem**, selecione um PNG ou JPEG, ajuste a largura e clique no ponto de inserção. Essa opção acrescenta uma marca visual. Para assinar o conteúdo com seu certificado, use **Assinar digitalmente**.

## Conferir uma assinatura

Abra o PDF assinado e clique em **Assinaturas digitais**. Selecione a assinatura para consultar o titular, o emissor, a integridade da versão assinada e se ela cobre o arquivo inteiro. Para uma cópia assinada pelo Mouratech PDF, o botão **Verificar** também confere a integridade do arquivo.

A conferência local não consulta a revogação do certificado. Para obter um relatório externo, selecione manualmente o **PDF digital assinado** no portal do ITI. O aplicativo processa os documentos no computador. O envio ao portal depende dessa ação. [Abrir o VALIDAR do ITI](https://validar.iti.gov.br/)

## Acrescentar texto, destacar e anotar

- **Inserir texto.** Digite o conteúdo, ajuste o tamanho e clique na página para conferir a posição. Essa ferramenta acrescenta texto à página.
- **Destacar um trecho.** Em **Ferramentas → Marca-texto**, arraste sobre a área desejada.
- **Adicionar ou ler uma nota.** Em **Ferramentas → Adicionar nota**, clique na página e escreva o comentário. Para consultá-lo depois, escolha **Ler notas da página**.
- **Excluir uma nota.** Em **Ferramentas → Remover nota da página**, selecione o comentário e clique em **Remover nota**. Para recuperar a última nota excluída, use **Desfazer** antes de salvar.

Use **Salvar** para gravar as alterações no arquivo aberto ou **Salvar como** para criar uma cópia. Conclua as edições antes de assinar digitalmente. O leitor bloqueia a edição de PDFs já assinados para preservar a assinatura.

## Unir, dividir ou reorganizar páginas

Abra **Ferramentas → Unir, dividir e organizar PDFs** e adicione os arquivos desejados.

- **Unir ou reorganizar.** Confira as miniaturas, use **Subir** e **Descer** para ordenar as páginas e remova as que deseja excluir. Clique em **Salvar PDF organizado** para criar o novo arquivo.
- **Extrair algumas páginas.** Selecione páginas com **Ctrl** ou um intervalo com **Shift**. Escolha **Extrair seleção** para reuni-las em um PDF.
- **Separar todas as páginas.** Escolha **Dividir por página** para criar uma pasta com um PDF por página.

A organização de páginas aceita documentos sem senha, assinaturas digitais ou campos de formulário.

## Proteger uma cópia com senha

Abra o PDF e escolha **Ferramentas → Proteger cópia com senha**. Digite e confirme a senha de abertura e salve a cópia. O arquivo protegido usa criptografia AES-256 e solicita a senha quando é aberto.

## Resolver problemas de assinatura

**Meu certificado não aparece.** Na mesma conta do Windows, abra `certmgr.msc` e confira **Pessoal → Certificados**. O aplicativo precisa de um certificado ICP-Brasil A1 RSA válido, com chave privada disponível. Se acabou de instalá-lo, clique em **Atualizar certificados**. A chave é usada pelo Windows, sem necessidade de exportar o PFX.

**O certificado aparece, mas não consigo assinar.** Confira se o carimbo está em uma área livre e se você marcou a confirmação. A assinatura também exige que o Windows reconheça a cadeia de autoridades emissoras. PDFs já assinados ou protegidos e documentos cuja página escolhida tenha rotação, anotações ou recorte especial podem impedir a assinatura nesta versão.

## Código-fonte e licença

O projeto usa C# e .NET 10 e gera assinaturas PAdES Baseline B. O pacote de código-fonte inclui as dependências e as licenças. O código-fonte desta instalação fica na pasta **Fonte** · [Licença GNU AGPLv3 do projeto](https://github.com/mouratech-udi/mouratech-pdf/blob/main/LICENSE.md)

Para compilar no Windows com o SDK .NET 10, execute estes comandos na pasta que contém `Mouratech.csproj`:

```powershell
dotnet restore --locked-mode -r win-x64
dotnet publish -c Release -r win-x64 --self-contained true -o ../publicado
```

Para executar o autoteste, abra a pasta `publicado` e use um nome de diretório de saída que ainda não exista. O teste usa documentos e certificado fictícios. O código de saída zero indica sucesso.

```powershell
$p = Start-Process -FilePath .\Mouratech.Assinador.exe -ArgumentList '--autoteste ensaio-local' -Wait -PassThru
$p.ExitCode
```
