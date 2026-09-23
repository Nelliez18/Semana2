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
