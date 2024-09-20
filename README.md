class Carro:
    def __init__(self, codigo, fabricante, modelo, cor, valor, ano):
        self.codigo = codigo
        self.fabricante = fabricante
        self.modelo = modelo
        self.cor = cor
        self.valor = valor
        self.ano = ano

    def calcular_parcelas(self):
        quantidade_parcelas = int(input("Digite a quantidade de parcelas: "))
        if quantidade_parcelas <= 0:
            print("A quantidade de parcelas deve ser maior que zero.")
            return
        valor_parcela = self.valor / quantidade_parcelas
        print(f"O valor de cada parcela será: R$ {valor_parcela:.2f}")

    def exibir_dados(self):
        print("Dados do Carro:")
        print(f"Código: {self.codigo}")
        print(f"Fabricante: {self.fabricante}")
        print(f"Modelo: {self.modelo}")
        print(f"Cor: {self.cor}")
        print(f"Valor: R$ {self.valor:.2f}")
        print(f"Ano: {self.ano}")

def main():
    # Coletar dados do carro
    codigo = input("Digite o código do carro: ")
    fabricante = input("Digite o fabricante: ")
    modelo = input("Digite o modelo: ")
    cor = input("Digite a cor: ")
    valor = float(input("Digite o valor: R$ "))
    ano = int(input("Digite o ano: "))

    # Criar um objeto Carro
    carro = Carro(codigo, fabricante, modelo, cor, valor, ano)

    # Exibir os dados do carro
    carro.exibir_dados()

    # Calcular parcelas
    carro.calcular_parcelas()

# Executar o programa
- 👋 Hi, I’m @brehmartins
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
brehmartins/brehmartins is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
