# Ideia principal para o trabalho

Aplicar conhecimentos de algoritmos matemáticos e pensamento computacional desenvolvendo um
simulador de meio de pagamento (SMP) em C. Para as operações de débito será cobrado 1% de
MDR (taxa da transação), e para cartão de crédito (somente a vista) será cobrado 5% de MDR. As
operações por Pix não terão desconto de MDR.
A arquitetura do SMP será composto de front-end e back-end. No front-end o requerido é somente
uma tela HTML (fica a critério do grupo o uso de css e javascript), contendo um campo númerico
de 6 digitos, o valor e o meio de pagamento. O back-end será um programa em C que receberá os 3
campos e deverá calcular o desconto (débito e crédito) e passar para uma rotina que irá grava um
arquivo JSON. Será disponibilizada a biblioteca unicsul.h (em C) que deverá ser incluída no
programa em C (back-end) contendo algumas rotinas, por exemplo, identificar a próxima data útil,
gravar arquivo JSON e etc.
## Este projeto visa a capacitação em:
### Pensamento computacional
### Lógica de negócios real
### Uso de bibliotecas
### Projeto de algoritmos
### Validação de dados
### Operações matemáticas & financeiras
### Manipulação de data e hora
projeto pode ser desenvolvido usando o IDE Devcpp
