# Mouratech PDF — Leitor e Assinador Digital

## Instalação com Windows Installer
Execute Mouratech-PDF-1.3.1-x64.msi com o usuário que utilizará o leitor. Procure Mouratech PDF no menu Iniciar. No Explorer, clique com o botão direito em um PDF, escolha Abrir com e selecione Mouratech PDF. A escolha de leitor padrão fica com o usuário. Próximos instaladores MSI com versão superior atualizam esta instalação. Uma versão antiga extraída de ZIP pode coexistir em outra pasta. Para remover a instalação MSI use Aplicativos instalados no Windows.

## Ferramentas do PDF
Para marcar uma área, escolha **Ferramentas → Marca-texto** e arraste sobre o trecho. Para anotar, escolha **Adicionar nota**, clique na página e digite o comentário. **Ler notas da página** mostra o conteúdo. Para excluir uma, use **Ferramentas → Remover nota da página**, selecione a nota e clique em **Remover nota**. A última exclusão pode ser desfeita antes de salvar. Use **Salvar** ou **Salvar como** para gravar as alterações.

**Unir, dividir e organizar PDFs** reúne as páginas em uma lista com prévia. Adicione arquivos, altere a ordem com **Subir** e **Descer** ou remova páginas. **Salvar PDF organizado** gera um novo arquivo. Para extrair várias páginas juntas, selecione-as com Ctrl ou Shift e escolha **Extrair seleção**. **Dividir por página** cria uma nova pasta com um PDF por página. Esta versão trabalha com páginas de documentos sem proteção, assinaturas digitais ou campos de formulário.

**Proteger cópia com senha** cria um novo PDF com criptografia AES-256. Informe e confirme a senha de abertura. O leitor solicita a senha ao abrir a cópia e permite consultá-la em modo de leitura.

## Buscar com Ctrl+F
Digite o texto e pressione Enter para localizar e avançar. Shift+Enter volta uma ocorrência. A busca indica a quantidade e destaca o trecho em amarelo. Esc fecha a busca. PDFs digitalizados precisam de uma camada de texto para permitir pesquisa.

## Assinar lote
Clique em Assinar lote e selecione os PDFs no disco. Revise cada documento, marque “Confirmo que desejo assinar este documento” e clique em Aprovar para o lote. O primeiro certificado aprovado vale para todo o lote. Você pode pular um documento ou cancelar antes da confirmação final. Depois de confirmar, cada cópia é gravada na pasta do original com o sufixo _assinado. Arquivos alterados desde a revisão e destinos existentes são preservados. Confira o resultado individual na janela final. O lote usa os arquivos salvos no disco.

A impressão física foi confirmada pelo usuário na estação da clínica na versão anterior.

## Instalação portátil
Em um Windows 10/11 de 64 bits compatível com .NET 10, extraia **todo** o ZIP para uma pasta local, por exemplo Documentos ➜ Aplicativos ➜ Mouratech. Abra **Mouratech.Assinador.exe**. O runtime está incluído. O pacote piloto não tem assinatura de editor Authenticode. Mantenha as DLLs junto ao executável.

Use o mesmo usuário do Windows em que o seu certificado A1 já está instalado. Em certmgr.msc, confira Pessoal ➜ Certificados, chave privada correspondente e cadeia confiável. O aplicativo usa o repositório Usuário Atual e o provedor criptográfico do Windows. A seleção exige RSA, política de certificado ICP-Brasil A1, validade atual e uso de chave compatível. A assinatura exige que o Windows consiga construir a cadeia com as autoridades já disponíveis.

## Ler, editar e imprimir
Abra um PDF pelo botão **Abrir**, pelo menu **Abrir com** do Windows ou passando o caminho ao executável. Clique nas miniaturas à esquerda para navegar. O rodapé mostra a página atual e o total. Sobre o PDF, gire a roda do mouse para cima para ampliar ou para baixo para reduzir, sem segurar Ctrl. Cada passo muda o zoom em 10 pontos percentuais. Sobre as miniaturas, a roda percorre a lista. Use o controle de zoom de 25% a 300%, **Ajustar página** para enquadrar a folha e **Miniaturas** para ocultar ou exibir a lateral.

Para rolar, segure o botão esquerdo sobre a página e arraste. Com a folha inteira visível na vertical, um arraste para cima avança uma página e um arraste para baixo volta. As barras de rolagem continuam disponíveis quando o conteúdo ultrapassa a janela.

Ao abrir um PDF assinado, use **Assinaturas digitais** na barra superior. Escolha a assinatura para ir à página do campo e consultar o titular, o emissor, a integridade da revisão e a cobertura do arquivo. A marca visual depende da aparência gravada no PDF. A verificação local de integridade não consulta revogação.

**Inserir texto** acrescenta texto com tamanho ajustável e quebras de linha à página escolhida. O texto já impresso no PDF permanece como está. **Assinar por imagem** aceita PNG e JPEG. Ajuste a largura, clique no ponto de inserção e confira a prévia antes de aplicar. Se mudar o texto ou o tamanho, clique de novo na página. A imagem é uma marca visual. Use **Assinar digitalmente** para vincular o certificado ao conteúdo, incluindo as alterações que estão em tela.

**Desfazer** remove a última inserção antes de salvar. **Salvar** grava as alterações no PDF aberto. **Salvar como** permite manter o original. PDFs assinados podem ser lidos, copiados e impressos. A edição fica bloqueada para preservar a assinatura. **Imprimir** usa a caixa de impressão do Windows para todas as páginas ou um intervalo. O papel impresso reproduz o conteúdo visual. A verificação criptográfica depende do arquivo digital.

## Assinar um documento
1. Escolha o documento PDF. Use uma pasta local de acesso restrito e fora de pastas sincronizadas para o fluxo confidencial.
2. Abra o arquivo no leitor, clique em **Assinar digitalmente** e confira a última página. Selecione o certificado que deseja usar. A seleção mostra o titular e a data de vencimento.
3. A sugestão inicial foi calibrada no PDF de referência de três páginas. Para ajustar, clique no centro da linha de assinatura ou na borda superior do nome. O carimbo ficará 4 pontos acima do clique. O contorno verde indica área livre. Em vermelho, o comando de assinatura fica bloqueado. O contorno é exclusivo da prévia.
4. Marque **Confirmo que desejo assinar este documento** e clique em **Assinar e salvar cópia**. A janela de destino sugere a mesma pasta e o sufixo **_assinado.pdf**. Você também pode escolher outra pasta ou outro nome. Uma cópia existente impede nova gravação. O programa também confere se o PDF aberto mudou desde a prévia.
5. Para conferir novamente, use **Verificar uma cópia**. A função aceita a assinatura individual criada por este aplicativo, verifica o conteúdo criptográfico e exige cobertura de todo o arquivo.

## Homologação na Multiclínica
Gere um laudo com paciente fictício no Ergo PC 5.1.1.18 e assine com o A1 instalado na estação do médico. Abra a cópia no leitor habitual e confira as três páginas. Compare conclusão, identificação e CRM. Para avaliação externa, envie manualmente **a cópia fictícia assinada** ao [VALIDAR do ITI](https://validar.iti.gov.br/). Confira o titular e o resultado no relatório de conformidade. Registre o resultado antes de liberar o fluxo clínico. O aplicativo não inicia esse envio.

## Implementação e limites do piloto
C# / .NET 10, Windows Forms x64. PAdES Baseline B via iText, SHA-256/RSA, assinatura de certificação DocMDP P=1 e gravação incremental. O carimbo visível diz “Assinado digitalmente”. Os dados do titular estão no certificado incorporado. A criação verifica assinatura, identidade e cobertura antes da publicação da cópia. A rotina local não consulta revogação nem fornece carimbo de tempo confiável ou validação de longo prazo. O usuário apresentou a aprovação do VALIDAR para uma assinatura individual produzida na clínica. A assinatura em lote desta versão foi testada com certificado de laboratório.

A prévia e a verificação de espaço usam PDFium a 216 dpi e exigem fundo branco, com margem de 2 pontos ao redor do retângulo. A conferência humana vincula a posição ao médico identificado. O piloto bloqueia documentos já assinados, criptografados e páginas finais com rotação, anotações ou geometria não suportada. Não há envio de laudos, registro clínico em log, monitoramento automático de pastas. O PDF original e certificados particulares ficam fora da distribuição.

## Projeto e reprodução
O diretório **Fonte** do pacote contém o projeto, o arquivo de dependências fixadas e o autoteste. Com o SDK .NET 10 no Windows, dentro de Fonte, execute:

```powershell
dotnet restore --locked-mode -r win-x64
dotnet publish -c Release -r win-x64 --self-contained true -o ../publicado
```

Para executar o autoteste na pasta do programa, escolha um diretório de saída novo:

```powershell
$p = Start-Process -FilePath .\Mouratech.Assinador.exe -ArgumentList '--autoteste ensaio-local' -Wait -PassThru
$p.ExitCode
```

O código 0 indica aprovação. O ensaio gera um par de PDFs fictícios e usa uma chave RSA efêmera. Exercita colisão, rejeição de certificado sem política A1, perfil PAdES, DocMDP, preservação dos bytes originais e detecção de alteração ou dados anexados. Não utiliza o repositório pessoal. É separado do teste de homologação descrito acima.

## Licenças
Esta edição piloto com fonte incluída utiliza iText sob AGPLv3. Consulte o texto da licença em Licencas. Para distribuição proprietária, reveja o licenciamento comercial do iText antes da entrega dessa modalidade. As demais dependências conservam suas licenças. [Licenciamento iText](https://itextpdf.com/how-buy)









