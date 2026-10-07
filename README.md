# Conversor FOPAG BB

Ferramenta local (sem servidor, sem backend) para converter os relatórios em PDF da folha de
pagamento — **BBGestaoMax** ou **Fortes** — em uma planilha XLSX pronta para importar na
**Folha de Pagamento (Fopag Digital)** do BB Digital PJ.

Todo o processamento acontece no navegador: o PDF nunca sai da máquina do usuário.

## Arquivos

- **`conversor_fopag_digital.html`** — o conversor. Selecione o tipo de arquivo, solte o PDF,
  confira os dados extraídos na tela e gere a planilha (`CPF`, `Agência com DV`, `Conta com DV`,
  `Valor`).
- **`Tutorial_Importar_Planilha_BBDigitalPJ.html`** — passo a passo de como importar a planilha
  gerada na tela de Folha de Pagamento do BB Digital PJ, com link para o vídeo tutorial.

## Como usar

Abra `conversor_fopag_digital.html` direto no navegador — não é necessário instalar nada nem
rodar um servidor.

## Stack

HTML + CSS + JavaScript puro, com [pdf.js](https://mozilla.github.io/pdf.js/) para leitura do PDF
e [SheetJS](https://sheetjs.com/) para gerar o XLSX, ambos carregados via CDN.
