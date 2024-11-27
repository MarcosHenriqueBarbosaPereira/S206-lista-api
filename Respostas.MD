# Respostas das Questões Teóricas

## **1. Os testes desenvolvidos são manuais ou automatizados?**

Esses testes foram desenvolvidos como scripts automatizados capazes de, por conta própria, realizar requisições em alguma API e validar os elementos da resposta que recebem.
Além disso, quando são executados, não é necessário fazer nenhuma inferência humana para validar quaisquer resultados, considerando que o próprio teste automatizado faz isso.
Desta forma, pode-se concluir que os testes desenvolvidos são testes autumatizados.

## **2. Alguns dos testes dessenvolvidos são teste Fim-a-Fim (End-to-End - E2E)?**

Testes E2E são responsáveis por testar de forma completa um fluxo de funcionamentos de um sistema completo.
Assim sendo, como estamos apenas validando as respostas obtidas para requisições feitas para uma API apenas, não tendo quaisquer testes para funcionalidades extras de um sistema hipotético que processe e/ou controle esses dados.
Conclui-se portanto que nenhum dos testes desenvolvidos é um teste E2E.

## **3. O que deve ser feito para os testes desenvolvidos funcionarem em modo regressão?**

Para o teste funcionar como teste de regressão, ele precisa ficar continuamente realizando verificações no código a cada vez que ocorre uma alteração ou desenvolvimento adicional, garantindo assim que a implementação de novas funcionalidades não causem a quebra nas funcionalidades já existentes. Considerando isso, os testes podem ser implementados junto a uma ferramenta de CI/CD, como o GitHub Actions estudado na disciplina de Engenharia de Software (C214). Diante disso, além dos testes automatizados, a execução deles sobre o código dessenvolvido também vai esstar automatizados, garantindo que todas as funcionalidades já existentes estejam funcionando propriamente quando qualquer alteração ocorra no código, garantindo assim uma verificação sobre regressão no código.