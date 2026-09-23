Classificador de Cliente
```python
# Em python
idade = int(input("Digite a idade do cliente: "))
renda = float(input("Digite a renda do cliente: "))

if renda <= 3000.0:
    categoria = "Bronze"
elif renda <= 6000.0:
    categoria = "Prata"
elif renda <= 12000.0:
    categoria = "Ouro"
else:
    categoria = "Diamante"

print(f"Categoria: {categoria}")

```
```portugol
// Em portugol
programa {
	funcao inicio() {
		inteiro idade
		real renda

		escreva("Digite a idade do cliente: ")
		leia(idade)
		escreva("Digite a renda do cliente: ")
		leia(renda)

		se (renda <= 3000.0) {
			escreva("Categoria: Bronze\n")
		} senao se (renda <= 6000.0) {
			escreva("Categoria: Prata\n")
		} senao se (renda <= 12000.0) {
			escreva("Categoria: Ouro\n")
		} senao {
			escreva("Categoria: Diamante\n")
		}
	}
}
```
Menu de Operações Matemáticas
```python
# Em python
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

print("\n--- MENU DE OPERAÇÕES ---\n1 - Soma\n2 - Subtração\n3 - Multiplicação\n4 - Divisão")
opcao = int(input("Escolha uma opção (1-4): "))

match opcao:
    case 1:
        print(f"Resultado: {num1 + num2}")
    case 2:
        print(f"Resultado: {num1 - num2}")
    case 3:
        print(f"Resultado: {num1 * num2}")
    case 4:
        if num2 != 0:
            print(f"Resultado: {num1 / num2}")
        else:
            print("Erro: Divisão por zero!")
    case _:
        print("Opção inválida!")
```
```portugol
// Em portugol
programa {
	funcao inicio() {
		real num1, num2, resultado
		inteiro opcao

		escreva("Digite o primeiro número: ")
		leia(num1)
		escreva("Digite o segundo número: ")
		leia(num2)

		escreva("\n--- MENU DE OPERAÇÕES ---\n")
		escreva("1 - Soma\n2 - Subtração\n3 - Multiplicação\n4 - Divisão\n")
		escreva("Escolha uma opção (1-4): ")
		leia(opcao)

		escolha (opcao) {
			caso 1:
				resultado = num1 + num2
				escreva("Resultado: ", resultado, "\n")
				pare
			caso 2:
				resultado = num1 - num2
				escreva("Resultado: ", resultado, "\n")
				pare
			caso 3:
				resultado = num1 * num2
				escreva("Resultado: ", resultado, "\n")
				pare
			caso 4:
				se (num2 != 0) {
					resultado = num1 / num2
					escreva("Resultado: ", resultado, "\n")
				} senao {
					escreva("Erro: Divisão por zero!\n")
				}
				pare
			caso contrario:
				escreva("Opção inválida!\n")
		}
	}
}
```
Análise de Números
```python
# Em python
soma = 0
maior = None
menor = None

for i in range(1, 6):
    numero = float(input(f"Digite o {i}º número: "))
    soma += numero
    
    if maior is None or numero > maior:
        maior = numero
    if menor is None or numero < menor:
        menor = numero

media = soma / 5

print(f"\nSoma: {soma}")
print(f"Média: {media:.2f}")
print(f"Maior valor: {maior}")
print(f"Menor valor: {menor}")
```
```portugol
// Em portugol
programa {
	funcao inicio() {
		real numero, soma = 0.0, media, maior = 0.0, menor = 0.0
		inteiro i

		para (i = 1; i <= 5; i++) {
			escreva("Digite o ", i, "º número: ")
			leia(numero)

			soma = soma + numero

			// Define o primeiro número lido como o maior e o menor inicial
			se (i == 1) {
				maior = numero
				menor = numero
			} senao {
				se (numero > maior) { maior = numero }
				se (numero < menor) { menor = numero }
			}
		}

		media = soma / 5

		escreva("\nSoma: ", soma)
		escreva("\nMédia: ", media)
		escreva("\nMaior valor: ", maior)
		escreva("\nMenor valor: ", menor, "\n")
	}
}
```
Sistema de Autenticação
```python
# Em python
senha_correta = "1234"
tentativas = 0

while tentativas < 3:
    senha_digitada = input("Digite a senha: ")
    tentativas += 1
    
    if senha_digitada == senha_correta:
        print("Acesso Permitido!")
        break
    else:
        print(f"Senha Incorreta. Tentativa {tentativas} de 3.")
else:
    print("Acesso Bloqueado após 3 erros.")
```
```portugol
// Em portugol
programa {
	funcao inicio() {
		cadeia senha_correta = "1234"
		cadeia senha_digitada
		inteiro tentativas = 0
		logico bloqueado = falso

		enquanto (tentativas < 3) {
			escreva("Digite a senha: ")
			leia(senha_digitada)
			tentativas = tentativas + 1

			se (senha_digitada == senha_correta) {
				escreva("Acesso Permitido!\n")
				pare
			} senao {
				escreva("Senha Incorreta. Tentativa ", tentativas, " de 3.\n")
				se (tentativas == 3) {
					bloqueado = verdadeiro
				}
			}
		}

		se (bloqueado) {
			escreva("Acesso Bloqueado após 3 erros.\n")
		}
	}
}
```
