# prova1python
Sistema de Gerenciamento de Frota
Este projeto tem como objetivo gerenciar diferentes tipos de veículos de uma frota e suas manutenções. Foi desenvolvido em Python, utilizando os conceitos de Herança, Encapsulamento e Polimorfismo.

Descrição das Classes:
# Classe Veiculo (superclasse): representa um veículo genérico.

Atributos:
marca (str)
modelo (str)
ano_fabricacao (int)
chassi (str)
cor (str)
quilometragem (float)

Métodos:
registrar_manutencao(tipo, custo) – Registra uma manutenção com o tipo e custo.
exibir_informacoes(detalhado) – Exibe informações resumidas ou detalhadas do veículo.

# Classe CarroPasseio (subclasse): representa um carro de passeio herda de Veiculo.

Atributo:
tipo_combustivel (str)

Métodos:
calcular_depreciacao(anos_uso, taxa_extra) – Calcula a depreciação do carro.
exibir_informacoes(detalhado) – Sobrescreve o método da superclasse para exibir também os atributos.

# Classe CaminhaoCarga (subclasse): representa um caminhão de carga herda de Veiculo.

Atributos adicionais:
capacidade_toneladas (float)
eixos (int)

Métodos:
registrar_vistoria(motivo, multa) – Exibe o motivo da vistoria e o valor da multa, se houver.
exibir_informacoes(detalhado) – Sobrescreve o método da superclasse para mostrar também os novos atributos.

# Exemplos de Execução
Criando um carro
carro = CarroPasseio("Chevrolet", "Camaro", 2020, "1234", "Amarelo", 45000, 4, "Gasolina")
carro.exibir_informacoes(detalhado=True)
carro.registrar_manutencao("Troca de óleo", 250)
carro.calcular_depreciacao(5, 1200)

Criando um caminhão
caminhao = CaminhaoCarga("Volvo", "Caminhão", 2018, "5678", "Preto", 150000, 25.5, 4)
caminhao.exibir_informacoes(detalhado=True)
caminhao.registrar_manutencao("Revisão geral", 3000)
caminhao.registrar_vistoria("Vistoria anual", 500)

# Nome: João Pedro Cabrera
Possui metodos adicionais inclementados para deixar o sistema mais completo.
Deve ser executado pelo arquivo main.py.
# Obrigado professor!!
