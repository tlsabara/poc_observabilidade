# poc_observabilidade

Esta é uma POC para aplicar ferramentas de observabilidade em projetos de desenvolvimento WEB.

## Idéa de trabalho

Aplciar as ferramentas em uma aplicaçao de microsserviços e em um monolito.

A aplicação é uma simples calculadora, e que consome endpoints externos.

Serão 5 serviços HTTP:
- API: Monolito, com os endpoints abertos.
- Calc_A: faz os calculos de soma e subtração.
- Calc_B: faz os calculos de divisão e multiplicação. Este serviço pode gerar erros.
- Ender_C: confere os calculos aplicados, pode receber chamada de A e B.
- Ender_D: confere os calculos aplicados, pode receber chamada de A e B. Este serviço pode gerar erros.
- Returner: Finaliza o calculo e retorna o resultado para a API.

