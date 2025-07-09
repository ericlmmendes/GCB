Gerador de Códigos de Barras
Descrição do Repositório GitHub
Um gerador de códigos de barras baseado na web que cria códigos CODE128 a partir de números fornecidos pelo usuário e os exporta como PDF. Desenvolvido com HTML, JavaScript, Tailwind CSS, jsPDF e JsBarcode.
Visão Geral
Este projeto é uma aplicação web que permite aos usuários gerar códigos de barras CODE128 a partir de uma lista de números inserida em uma área de texto. Os códigos de barras são organizados em um layout de grade em páginas de tamanho A4 e exportados como PDF usando a biblioteca jsPDF. A aplicação possui um design responsivo com Tailwind CSS, uma barra de progresso para feedback durante a geração e um botão flutuante do WhatsApp para suporte. O projeto também inclui suporte para processamento de arquivos XLSX (embora não esteja totalmente implementado no código fornecido).
Funcionalidades

Geração de códigos de barras CODE128 a partir de números inseridos pelo usuário.
Exportação dos códigos de barras para um PDF baixável em formato A4.
Interface responsiva com Tailwind CSS.
Barra de progresso para acompanhar o processo de geração.
Botão flutuante do WhatsApp para suporte.
Tratamento de erros para entradas inválidas de códigos de barras.

Instalação
Para executar o projeto localmente, siga estas etapas:

Clonar o repositório:
git clone https://github.com/seu-usuario/gerador-codigos-barras.git
cd gerador-codigos-barras


Servir a aplicação:Como é uma aplicação web do lado do cliente, você pode servi-la com um servidor HTTP simples. Por exemplo, usando Python:
python -m http.server 8000

Em seguida, abra http://localhost:8000 no seu navegador.

Dependências:O projeto utiliza bibliotecas hospedadas em CDNs, portanto, não é necessário instalar nada adicional:

Tailwind CSS
Font Awesome
JsBarcode
jsPDF

Nota: O processamento de arquivos XLSX requer a biblioteca SheetJS, que é referenciada, mas não incluída no código fornecido. Para habilitar suporte a XLSX, adicione:
<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>



Uso

Abra a aplicação em um navegador web.
Insira os números dos códigos de barras na área de texto, um por linha.
Clique no botão "Gerar PDF de Códigos de Barras" para criar o PDF.
Se nenhum código for fornecido, um alerta solicitará que você insira pelo menos um código.
Uma barra de progresso mostrará o andamento da geração, e o PDF será baixado automaticamente como barcodes.pdf.

Estrutura do Projeto

index.html: O arquivo HTML principal que contém a interface e a lógica JavaScript.
JavaScript:
Geração de códigos de barras usando JsBarcode e jsPDF.
Suporte opcional para processamento de arquivos XLSX com SheetJS (não totalmente implementado).


CSS: Estilizado com Tailwind CSS via CDN.

Contribuição
Contribuições são bem-vindas! Para contribuir:

Faça um fork do repositório.
Crie uma nova branch (git checkout -b funcionalidade/sua-funcionalidade).
Faça suas alterações e commit (git commit -m "Adiciona sua funcionalidade").
Envie para a branch (git push origin funcionalidade/sua-funcionalidade).
Abra um pull request.

Licença
© 2025 ERICLM. Todos os direitos reservados.
Contato
Para suporte ou dúvidas, entre em contato via WhatsApp em +55 11 93008-9968.
