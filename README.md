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

      ```python
      # Algoritmo Sistema de Avaliação Escolar
      # Declaração de Variáveis
      
      nota1 = float(input('Digite a primeira nota: '))
      nota2 = float(input('Digite a segunda nota: '))
      nota3 = float(input('Digite a terceira nota: '))
      
      media = float(nota1 + nota2 + nota3) / 3
      
      if media >= 7:
        print('Parabéns, você foi aprovado!')
      elif media >= 3:
        print('Você fará a Prova Final, não desista agora!')
      
        nota_exame = 6.0 * 2 - media
        print(f'Para ser aprovado no exame, você precisa tirar pelo menos {nota_exame:.2f}.')
      else:
        print('Sentimos muito, mas você foi reprovado...')
      ```
<br>

2. **Faça um programa que receba dois números e mostre o maior.**
 
      ```python
      # Algoritmo Mostra Maior
      # Declaração de Variáveis

      n1 = int(input('Digite o primeiro número: '))
      n2 = int(input('Digite o segundo número: '))
      
      if n1 > n2:
        n = n1
      else:
        n = n2
      
      print(f'O maior número é: {n}')
      ```
<br> 

3. **Faça um programa que receba três números e mostre-os em ordem crescente.**

      ```python
      # Algoritmo Mostra Crescente
      # Declaração de Variáveis
      
      n1 = int(input('Digite o primeiro número: '))
      n2 = int(input('Digite o segundo número: '))
      n3 = int(input('Digite o terceiro número: '))
      
      if n1 <= n2 <= n3:
          print(f"A ordem crescente é: {n1}, {n2} e {n3}")
      elif n1 <= n3 <= n2:
          print(f"A ordem crescente é: {n1}, {n3} e {n2}")
      elif n2 <= n1 <= n3:
          print(f"A ordem crescente é: {n2}, {n1} e {n3}")
      elif n2 <= n3 <= n1:
          print(f"A ordem crescente é: {n2}, {n3} e {n1}")
      elif n3 <= n1 <= n2:
          print(f"A ordem crescente é: {n3}, {n1} e {n2}")
      else:
          print(f"A ordem crescente é: {n3}, {n2} e {n1}")
      ```
<br>
 
4. **Faça um programa que receba três números obrigatoriamente em ordem crescente e um quarto número que não siga esta regra. Mostre, em seguida, os quatro números em ordem decrescente.**

      ```python
      # Algoritmo Mostra Decrescente
      # Declaração de Variáveis
      
      n1 = int(input('Digite o primeiro número: '))
      n2 = int(input('Digite o segundo número em ordem crescente: '))
      n3 = int(input('Digite o terceiro número em ordem crescente: '))
      n4 = int(input('Digite um número qualquer: '))
      
      if n1 <= n2 <= n3:
        if n3 >= n4:
          print(f'A ordem decrescente é: {n3}, {n2}, {n1} e {n4}')
        else:
          print('O quarto número não segue a regra de ordem crescente.')
      else:
        print('Os três primeiros números não estão em ordem crescente.')
      ```
<br>

5. **Faça um programa que receba o dia o mês e o ano e mostre nos seguintes formatos: dia/mês/ano - mês por extenso. (ex: 19/03/2020 -> 19 de março de 2020).**

      ```python
      # Algoritmo Formatador de Datas
      # Declaração de Variáveis
      
      dia = int(input('Digite o dia: '))
      mes = int(input('Digite o mes: '))
      ano = int(input('Digite o ano: '))
      
      meses = {
          1: 'janeiro',
          2: 'fevereiro',
          3: 'março',
          4: 'abril',
          5: 'maio',
          6: 'junho',
          7: 'julho',
          8: 'agosto',
          9: 'setembro',
          10: 'outubro',
          11: 'novembro',
          12: 'dezembro'
      }
      
      if mes >= 1 and mes <= 12:
        print(f'{dia} de {meses[mes]} de {ano}')
      else:
        print('Mês inválido. Insira um valor entre 1 e 12.')
      ```
<br>

6. **Faça um programa que receba o código correspondente ao cargo de um funcionário e seu salário atual e mostre o cargo, o valor do aumento e seu novo salário. Os cargos estão na tabela a seguir:**<br>

      | Código | Cargo | Percentual |
      |----------|----------|----------|
      | 1 | Escriturário  | 50%  |
      | 2 | Secretário | 35%  |
      | 3 | Caixa  | 20%  |
      | 4 | Gerente  | 10%  |
      | 5 | Diretor  | Não tem aumento  |

      ```python
      # Calculadora de Aumento Salarial
      # Declaração de Variáveis
      
      codigo = int(input('Digite o código correspondente ao cargo (1 a 5): '))
      salario_atual = float(input('Digite o salário atual do funcionário: '))
      
      if codigo == 1:
        cargo = 'Escriturário'
        percentual_aumento = 0.5
      elif codigo == 2:
        cargo = 'Secretário'
        percentual_aumento = 0.35
      elif codigo == 3:
        cargo = 'Caixa'
        percentual_aumento = 0.2
      elif codigo == 4:
        cargo = 'Gerente'
        percentual_aumento = 0.1
      elif codigo == 1:
        cargo = 'Diretor'
        percentual_aumento = 0
      else:
        print('Código inválido. Por favor, insira um valor entre 1 e 5.')
      
      aumento = salario_atual * percentual_aumento
      novo_salario = salario_atual + aumento
      
      print(f'\nCargo: {cargo}')
      print(f'Valor do aumento: R$ {aumento:.2f}')
      print(f'Novo salário: R$ {novo_salario:.2f}')
      ```
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
   
      ```python
      # Algoritmo Calculadora de Salário com Bonificação e Auxílio-Escola
      # Declaração de Variáveis
      
      salario = float(input('Digite o salário do funcionário: '))
      
      if salario <= 500:
        bonificacao = salario * 0.05
      elif 500 < salario <= 1200:
        bonificacao = salario * 0.12
      else:
        bonificacao = 0
      
      if salario <= 600:
        auxilio_escola = 150
      else:
        auxilio_escola = 100
      
      novo_salario = salario + bonificacao + auxilio_escola
      
      print(f'\nSalário inicial: R$ {salario:.2f}')
      print(f'Bonificação: R$ {bonificacao:.2f}')
      print(f'Auxílio-escola: R$ {auxilio_escola:.2f}')
      print(f'Novo salário: R$ {novo_salario:.2f}')
      ```
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
    
      ```python
      # Algoritmo Calculadora para Equação Quadrática
      # Declaração de Variáveis
      
      def raiz(numero):
        return numero ** 0.5
      
      a = float(input('Digite o valor de a (a deve ser diferente de zero): '))
      b = float(input('Digite o valor de b: '))
      c = float(input('Digite o valor de c: '))
      
      if a == 0:
        print('O coeficiente a deve ser diferente de zero.')
      else:
        delta = b ** 2 - 4 * a * c
      
        if delta < 0:
          print('Não existe raiz real.')
        elif delta == 0:
          x = -b / (2 * a)
          print(f'Existe uma raiz real: x = {x}')
        else:
          x1 = (-b + raiz(delta)) / (2 * a)
          x2 = (-b - raiz(delta)) / (2 * a)
          print(f'Existem duas raízes reais: x1 = {x1}, x2 = {x2}')
      ```
<br>

9. **Dados três valores X, Y e Z, verificar se eles podem ser os comprimentos dos lados de um triângulo e, se forem, verificar se o um triângulo equilátero, isósceles ou escaleno. Se eles não formarem um triângulo escrever uma mensagem. Considerar que:**<br>

      ```python
      # O comprimento de cada lado de um triângulo é menor que a soma dos outros dois lados;
      # Chama-se triângulo equilátero o triângulo que tem três lados iguais;
      # Chama-se triângulo isósceles o triângulo que tem o comprimento de dois lados iguais;
      # Chama-se triângulo escaleno o triângulo que tem os três lados diferentes.
      ```

      ```python
      # Algoritmo Verificador e Classificador de Triângulos
      # Declaração de Variáveis
      
      x = float(input('Digite o comprimento do lado X: '))
      y = float(input('Digite o comprimento do lado Y: '))
      z = float(input('Digite o comprimento do lado Z: '))
      
      if x + y > z and x + z > y and y + z > x:
        if x == y == z:
          tipo_triangulo = 'equilátero'
        elif x == y or x == z or y == z:
          tipo_triangulo = 'isósceles'
        else:
          tipo_triangulo = 'escaleno'
      
        print(f'\nOs lados formam um triângulo {tipo_triangulo}.')
      else:
        print('\nOs lados não formam um triângulo.')
      ```
<br>

10. **Faça um programa que receba:**
      ```python
      # O código sempre válido de um produto comprado, ou seja, um número inteiro entre l e 10;
      # O peso do produto em quilos;
      # O  código sempre válido do país de origem, ou seja, um número inteiro entre 1 e 3.
      ```

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

      Calcule e mostre:<br>
      &nbsp;&nbsp;&nbsp;1. O peso do produto convertido em gramas.<br>
      &nbsp;&nbsp;&nbsp;2. O preço total do produto comprado.<br>
      &nbsp;&nbsp;&nbsp;3. O valor do imposto, sabendo-se que ele é cobrado sobre o preço total do produto comprado e depende do país de origem.<br>
      &nbsp;&nbsp;&nbsp;4. O valor total, preço total do produto mais imposto.<br>

      ```python
      # Algoritmo Calculadora de Preço Total de Produto com Imposto
      # Declaração de Variáveis
      
      codigo_produto = int(input('Digite o código do produto (1 a 10): '))
      peso_quilos = float(input('Digite o peso do produto em quilogramas: '))
      codigo_pais = int(input('Digite o código do país de origem (1 a 3): '))
      
      peso_gramas = peso_quilos * 1000
      
      if 1 <= codigo_produto <= 4:
          preco_grama = 10
      elif 5 <= codigo_produto <= 7:
          preco_grama = 25
      elif 8 <= codigo_produto <= 10:
          preco_grama = 35
      else:
          print('Código do produto inválido. Por favor, insira um valor entre 1 e 10.')
          exit()
      
      preco_total = peso_gramas * preco_grama
      
      if codigo_pais == 1:
          taxa_imposto = 0
      elif codigo_pais == 2:
          taxa_imposto = 0.15
      elif codigo_pais == 3:
          taxa_imposto = 0.25
      else:
          print('Código do país de origem inválido. Por favor, insira um valor entre 1 e 3.')
          exit()
      
      valor_imposto = preco_total * taxa_imposto
      valor_total = preco_total + valor_imposto
      
      print(f'\nPeso do produto em gramas: {peso_gramas} g')
      print(f'\nPreço total do produto: R$ {preco_total:.2f}')
      print(f'\nValor do imposto: R$ {valor_imposto:.2f}')
      print(f'\nValor total: R$ {valor_total:.2f}')
      ```
