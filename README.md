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
