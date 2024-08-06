# Calculadora.py

# 2 Números de entrada de usuário

num1 = input("digite o primeiro número: ")
num2 = input("digite o segundo número: ")


# Conversão de valores recebidos para (int)

num1 = int(num1)
num2 = int(num2)

# Converta as entradas para int ou float (função)
def convert_to_number(value):
    try:
        # converta para inteiro
        return int(value)
    except ValueError:
      # se der erro, tentamos converter para float
      return float(value)

  # Converte as entradas:
  num1 = convert_to_number(num1)
  num2 = convert_to_number(num2)

  # Operações matemáticas:
  # Soma, Subtração, Multiplicação e Divisão
  soma = num1 + num2
  subtracao = num1 - num2
  multiplicacao = num1 * num2
  divisao = num1 / num2

  # Solicitar ao usuário qual operação deseja realizar
  print("qual operação você deseja fazer?")
  print("1 - Soma")
  print("2 - Subtração")
  print("3 - Multiplicação")
  print("4 - Divisão")
  operacao = input("Digite o número da operação desejada: ")

  # Resultado da operação matemática
  if (op == "1"):
    print(num1, "+", num2, " = ", num1 + num2)
    elif (op == "2"):
      print(num1, "-", num2, " = ", num1 - num2)
    elif (op == "3"):
      print(num1, "/", num2, " = ", num1 / num2)
    elif (op == "4"):
      print(num1, "*", num2, " = ", num1 * num2)
    else:
      print("operação inválida")

  # Realiza a operação escolhida
  Resultado = realizar_operacao(num1, num2, operacao)

  # Exibe o resultado da operação
  print("Resultado: ", Resultado)

  # O usuario deseja fazer outra op?
  continuar = input("deseja realizar mais operações? (s/n): ")
  if continuar.lower() != 's':
    break

    print("projeto finalizado. ")
