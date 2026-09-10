# Principais Regras de Negócio

## Estrutura Obrigatória do Projeto

O projeto deverá seguir a seguinte estrutura de diretórios e arquivos:

```text
projeto/
│
├── server.js
│
├── public/
│   ├── index.html
│   │
│   ├── css/
│   │   └── arquivos CSS externos (se houver)
│   │
│   ├── js/
│   │   └── arquivos JavaScript externos (se houver)
│   │
│   └── images/
│       └── arquivos de imagem (se houver)
│
├── cprogram/
│   └── programas em C (código-fonte e binários)
│
└── log/
    └── arquivos JSON gerados pelo sistema
```

## Regras do Backend

O backend deverá implementar as regras relacionadas aos meios de pagamento, cálculo financeiro, validação e armazenamento das informações.

### Meios de Pagamento

| Meio de pagamento | Taxa de MDR |
| ----------------- | ----------: |
| Débito            |          1% |
| Crédito à vista   |          5% |
| Pix               |          0% |

**MDR (Merchant Discount Rate)** é a taxa cobrada sobre uma transação.

### Validação e Processamento

* O campo numérico deverá aceitar no máximo **3 dígitos** no backend.
* O sistema deverá realizar o **cálculo do desconto referente ao MDR**.
* O sistema deverá calcular o **valor líquido** após a aplicação do MDR.
* As informações processadas deverão ser **armazenadas em arquivos JSON**.
* O uso de **JSON é obrigatório** no projeto.
* O sistema deverá possuir rotinas para processamento de informações, como, por exemplo:

  * Identificação do próximo dia útil;
  * Registro das informações da transação em um arquivo JSON.

### Requisitos Avaliados

O projeto deverá demonstrar a aplicação dos seguintes conceitos:

* Pensamento computacional;
* Lógica de programação;
* Utilização de bibliotecas;
* Desenvolvimento de algoritmos;
* Validação de dados;
* Matemática e conceitos financeiros;
* Manipulação de data e hora.

> **IDE obrigatória:** o projeto deverá ser desenvolvido utilizando a IDE **Dev-C++** para os programas em C.

## Regras do Frontend

O frontend deverá ser desenvolvido obrigatoriamente utilizando **HTML**. O uso de **CSS é opcional**.

### Campos e Validações

* Os campos numéricos deverão aceitar no máximo **6 dígitos** no frontend.
* O sistema deverá permitir a entrada de:

  * Valor da compra/doação;
  * Meio de pagamento;
  * Código do benfeitor.
* O **código do benfeitor não poderá aceitar o valor 0 (zero)**.

Exemplo de valor inválido:

```text
0000000
```

## Informações Armazenadas no JSON

Cada registro deverá armazenar as seguintes informações:

* **Data da compra/doação**;
* **Hora da compra/doação**;
* **Meio de pagamento**;
* **Valor da compra/doação**;
* **Valor do MDR**;
* **Valor líquido**;
* **Data do crédito**.

## Objetivo do Projeto

O projeto tem como objetivo desenvolver um sistema capaz de processar transações de compra/doação, aplicando as regras de negócio definidas para cada meio de pagamento, realizando os cálculos financeiros necessários, validando os dados fornecidos pelo usuário e armazenando os resultados em arquivos JSON.
