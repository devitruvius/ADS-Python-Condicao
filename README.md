# Aplicando Conceitos das Estruturas de Condição em Python

Este repositório contém exemplos de código em Python que aplicam conceitos das estruturas de condição. Os códigos foram desenvolvidos como parte das atividades da disciplina de Fundamentos de Algoritmo do curso de Análise e Desenvolvimento de Sistemas (ADS) pela Universidade Federal do Cariri (UFCA). O objetivo principal do cumprimento destas atividades foi fornecer uma prática sólida e consolidar os conceitos fundamentais relacionados às estruturas condicionais em Python, promovendo a compreensão e o aprimoramento das habilidades de programação nessa linguagem.

## Estrutura do Repositório

A estrutura do repositório foi organizada para proporcionar uma experiência de navegação eficiente e facilitar a revisão dos códigos. Cada bloco de atividade está representada por um tópico, dentro do qual você encontrará os repositórios dedicados às atividades desenvolvidas.

## Atividades

1. **Faça um programa que receba três notas de um aluno, calcule e mostre a média aritmética e a mensagem que segue a tabela abaixo. Para alunos de exame, calcule e mostre a nota que devera ser tirada no exame para aprová-lo, considerando que a média no exame é 6.0.**<br>

      | Média Aritmética | Mensagem |
      |----------|----------|
      | 0,0 ~ 3,0 | Reprovado  |
      | 3,0 ~ 7,0 | Exame |
      | 7,0 ~ 10,0 | Aprovado  |

   - [Sistema de Avaliação Escolar](https://github.com/devitruvius/algoritmo_sistema_avaliacao_escolar/blob/main/algoritmo_sistema_avaliacao_escolar.py)
<br>

2. **Faça um programa que receba dois números e mostre o maior.**
 
   - [Sistema de Identificação do Maior Número](https://github.com/devitruvius/algoritmo_mostra_maior/blob/main/algoritmo_mostra_maior.py)
<br> 

3. **Faça um programa que receba três números e mostre-os em ordem crescente.**

    - [Sistema de Ordenação Crescente](https://github.com/devitruvius/algoritmo_mostra_crescente/blob/main/algoritmo_mostra_crescente.py)
<br>
 
4. **Faça um programa que receba três números obrigatoriamente em ordem crescente e um quarto número que não siga esta regra. Mostre, em seguida, os quatro números em ordem decrescente.**

   - [Sistema de Ordenação Decrescente](https://github.com/devitruvius/algoritmo_mostra_decrescente/blob/main/algoritmo_mostra_decrescente.py)
<br>

5. **Faça um programa que receba o dia o mês e o ano e mostre nos seguintes formatos: dia/mês/ano - mês por extenso. (ex: 19/03/2020 -> 19 de março de 2020).**

    - [Sistema de Formatação de Datas](https://github.com/devitruvius/algoritmo_formatador_datas/blob/main/algoritmo_formatador_datas.py)
<br>

6. **Faça um programa que receba o código correspondente ao cargo de um funcionário e seu salário atual e mostre o cargo, o valor do aumento e seu novo salário. Os cargos estão na tabela a seguir:**<br>

      | Código | Cargo | Percentual |
      |----------|----------|----------|
      | 1 | Escriturário  | 50%  |
      | 2 | Secretário | 35%  |
      | 3 | Caixa  | 20%  |
      | 4 | Gerente  | 10%  |
      | 5 | Diretor  | Não tem aumento  |

   - [Sistema de Ajuste Salarial](https://github.com/devitruvius/algoritmo_calculadora_aumento_salarial/blob/main/algoritmo_calculadora_aumento_salarial.py)
<br>

7. **Faça um programa que receba o salário de um funcionário, calcule e mostre o novo salário desse funcionário, acrescido de bonificação e de auxílio-escola.**<br>

      | Salário | Bonificação |         
      |----------|----------|
      | Até R$ 500,00 | 5% do Salário  |
      | Entre R$ 500,00 e R$ 1.200,00 | 12% do Salário |
      | Acima de R$ 1.200,00 | Sem bonificação  |

   
      | Salário | Auxílio-Escola |         
      |----------|----------|
      | Até R$ 600,00 | R$ 150,00  |
      | Mais que R$ 600,00 | R$ 100,00 |
   
   - [Sistema de Cálculo de Salário com Bonificação e Auxílio-Escola](https://github.com/devitruvius/algoritmo_calculadora_salario_bonificacao_auxilio-escola/blob/main/algoritmo_calculadora_salario_bonificacao_auxilio-escola.py)
<br>

8. **Faça um programa para resolver equações do 2º. grau. (utilize a função RAIZ para a raiz quadrada).**

```python
# ax² + bx + c = 0
# A variável 'a' deve ser diferente de zero.
# Δ = b² - 4 * a * c
# Δ < 0 → não existe raiz real
# Δ = 0 → existe uma raiz real
# x = (-b)/(2 * a)
# Δ > 0 → existem duas raízes reais
# x1 = (-b + √Δ)/(2 * a)
# x2 = (-b - √Δ)/(2 * a)
```
    
  - [Calculadora de Equação Quadrática](https://github.com/devitruvius/algoritmo_calculadora_equacao_quadratica/blob/main/algoritmo_calculadora_equacao_quadratica.py)
<br>

9. **Dados três valores X, Y e Z, verificar se eles podem ser os comprimentos dos lados de um triângulo e, se forem, verificar se o um triângulo equilátero, isósceles ou escaleno. Se eles não formarem um triângulo escrever uma mensagem. Considerar que:**
    - O comprimento de cada lado de um triângulo é menor que a soma dos outros dois lados;
    - Chama-se triângulo equilátero o triângulo que tem três lados iguais;
    - Chama-se triângulo isósceles o triângulo que tem o comprimento de dois lados iguais;
    - Chama-se triângulo escaleno o triângulo que tem os três lados diferentes. 

    - [Verificador e Classificador de Triângulos](https://github.com/devitruvius/algoritmo_verificador_classificador_triangulos/blob/main/algoritmo_verificador_classificador_triangulos.py)
<br>

10. **Faça um programa que receba:**
    - O código de um produto comprado, supondo que a digitação do código do produto seja sempre válida, ou seja, um número inteiro entre l e 10;
    - O peso do produto em quilos;
    - O  código do país de origem, supondo que a digitação do código do país seja sempre válida, ou seja, um número inteiro entre 1 e 3.

      | Código do País de Origem | Imposto |         
      |----------|----------|
      | 1 | 0%  |
      | 2 | 15% |
      | 3 | 25% |

      | Código do Produto | Preço por Grama |         
      |----------|----------|
      | 1 a 4 | 10  |
      | 5 a 7 | 25 |
      | 8 a 10 | 35 |

Calcule e mostre:
   - O peso do produto convertido em gramas.
   - O preço total do produto comprado.
   - O valor do imposto, sabendo-se que ele é cobrado sobre o preço total do produto comprado e depende do país de origem.
   - O valor total, preço total do produto mais imposto.

   - [Calculadora de Preço Total com Imposto para Produtos](https://github.com/devitruvius/algoritmo_calculadora_preco_produto_com_imposto/blob/main/algoritmo_calculadora_preco_produto_com_imposto.py)
