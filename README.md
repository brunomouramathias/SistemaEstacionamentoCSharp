# SistemaEstacionamentoCSharp
Desafio de projeto .NET - Sistema de um Estacionamento

# 🚗 Sistema de Estacionamento - Trilha .NET - Fundamentos

Este repositório contém o desafio de projeto proposto na trilha de Fundamentos da .NET da DIO. O objetivo é consolidar os conhecimentos adquiridos no módulo, desenvolvendo um sistema para gerenciar veículos em um estacionamento.

---

## 📝 Desafio de Projeto

Você foi contratado para desenvolver um sistema que será utilizado em um estacionamento para gerenciar os veículos estacionados e realizar operações como:

- Adicionar um veículo.
- Remover um veículo (e calcular o valor total do período estacionado).
- Listar todos os veículos estacionados.

---

## 🛠️ Especificações Técnicas

### Classe: `Estacionamento`

O sistema deverá incluir uma classe chamada `Estacionamento`, conforme representado no diagrama abaixo:

![Diagrama de classe Estacionamento](diagrama_classe_estacionamento.png)

### Variáveis da Classe:

1. **`precoInicial`** (decimal): Representa o valor inicial cobrado ao estacionar um veículo.
2. **`precoPorHora`** (decimal): Representa o valor cobrado por hora de permanência.
3. **`veiculos`** (`List<string>`): Lista contendo as placas dos veículos estacionados.

### Métodos da Classe:

1. **`AdicionarVeiculo`**
   - Receber a placa do veículo digitada pelo usuário.
   - Adicionar a placa à lista de veículos estacionados (`veiculos`).

2. **`RemoverVeiculo`**
   - Verificar se um veículo está estacionado (pela placa informada).
   - Solicitar o número de horas que o veículo permaneceu no estacionamento.
   - Calcular o valor total utilizando a fórmula:
     ```
     Valor Total = precoInicial + (precoPorHora * horas)
     ```
   - Remover o veículo da lista e exibir o valor total ao usuário.

3. **`ListarVeiculos`**
   - Exibir uma lista de todos os veículos estacionados atualmente.
   - Caso a lista esteja vazia, exibir a mensagem: `"Não há veículos estacionados"`.

---

## 📋 Menu Interativo

O programa principal apresenta um menu interativo para o usuário com as seguintes opções:

1. **Cadastrar veículo** – adiciona um veículo ao sistema.
2. **Remover veículo** – remove um veículo estacionado e calcula o valor total.
3. **Listar veículos** – mostra todos os veículos atualmente estacionados.
4. **Encerrar** – finaliza o programa.

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
- [.NET SDK 6.0](https://dotnet.microsoft.com/download) instalado na máquina.

### Passos para executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/SeuUsuario/DesafioEstacionamento.git
   cd DesafioEstacionamento
   ```
2. Compile o projeto:
   ```bash
   dotnet build
   ```
3. Execute o programa:
   ```bash
   dotnet run
   ```

---

## ✍️ Autor Original

Projeto desenvolvido como parte do desafio da [Digital Innovation One (DIO)](https://www.dio.me/).

---

## ✍️ Desenvolvedor

O projeto foi enriquecido por [Bruno Moura Mathias](https://github.com/BrunoMouraMathias), que contribuiu para sua melhoria e documentação.

---
