## ClearBank - Análise de Transações Financeiras
### Descrição

Projeto desenvolvido em Python para leitura, validação, análise e geração de relatórios a partir de um arquivo CSV contendo transações financeiras.

O sistema realiza a limpeza dos dados, calcula métricas mensais, identifica transações suspeitas e exporta os resultados para um arquivo JSON.

### Funcionalidades
Leitura de arquivo CSV utilizando o módulo nativo csv
Validação e limpeza dos dados
Tratamento de erros com try/except
Conversão e manipulação de datas com datetime
Cálculo de métricas financeiras por mês
Identificação de transações suspeitas
Exibição de relatório formatado no terminal
Exportação do relatório para arquivo JSON

### Estrutura do Projeto
transacoes.csv → arquivo de entrada com as transações
relatorio.json → arquivo gerado automaticamente com o resumo dos dados
ClearBank.ipynb → notebook principal do projeto

### Regras de Validação

Uma transação é considerada inválida quando:

O campo id está vazio ou não é numérico
O campo cliente_id está vazio
A data não está no formato AAAA-MM-DD
O tipo é diferente de credito ou debito
O valor não é numérico ou é menor ou igual a zero

### Transações Suspeitas

São consideradas suspeitas todas as transações com valor superior a:

LIMITE_SUSPEITO = 10000.00

### Como Executar
Faça upload do arquivo transacoes.csv.
Abra o notebook ClearBank.ipynb no Google Colab.
Execute todas as células na ordem.
Consulte o relatório exibido no terminal.
Verifique o arquivo relatorio.json gerado automaticamente.

### Tecnologias Utilizadas
Python 3
csv
json
datetime
Autor

Felipe Vidal
