# POO Desafio - Modelagem do iPhone

Este projeto foi desenvolvido como parte de um desafio de Programação Orientada a Objetos (POO). O objetivo é modelar e implementar as funcionalidades de um iPhone, abrangendo as capacidades de **Reprodutor Musical**, **Aparelho Telefônico** e **Navegador na Internet**, utilizando interfaces e classes em Java.

---

## 📋 Funcionalidades

O projeto implementa as seguintes funcionalidades:

### **Reprodutor Musical**
- `tocar()`: Inicia a reprodução de uma música.
- `pausar()`: Pausa a música em reprodução.
- `selecionarMusica(String musica)`: Seleciona uma música para reprodução.

### **Aparelho Telefônico**
- `ligar(String numero)`: Realiza uma chamada para o número informado.
- `atender()`: Atende uma chamada.
- `iniciarCorreioVoz()`: Inicia o correio de voz.

### **Navegador na Internet**
- `exibirPagina(String url)`: Exibe a página da URL informada.
- `adicionarNovaAba()`: Adiciona uma nova aba no navegador.
- `atualizarPagina()`: Atualiza a página atual.

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
- Java Development Kit (JDK) instalado (versão 8 ou superior).
- Terminal ou IDE (como Visual Studio Code) configurado para compilar e executar projetos Java.

### Passos para Execução

1. **Clone ou baixe o projeto**:
  - Certifique-se de que todos os arquivos `.java` estão no mesmo diretório.

2. **Abra o terminal no diretório do projeto**:
   

3.  **Compile os arquivos Java:**
   - javac *.java

4. **Execute o programa principal:**
   - java Main

5. **Saída esperada: O programa exibirá no terminal as mensagens simulando as funcionalidades do iPhone, como:** 

    - Reproduzindo música...
    - Música pausada.
   - Música selecionada: Imagine - John Lennon
   - Ligando para: 123456789
   - Atendendo chamada...
   - Iniciando correio de voz...
   - Exibindo página: https://www.google.com
   - Nova aba adicionada.
   - Página atualizada.

---
## 📚 Conceitos Aplicados

### Programação Orientada a Objetos (POO):


   - Uso de interfaces para definir contratos de funcionalidades.
   - Implementação de polimorfismo ao criar uma classe que implementa múltiplas interfaces.

### Boas Práticas de Código:

   - Separação de responsabilidades em diferentes arquivos.
   - Uso de métodos claros e bem definidos.

---
### 🖥️ Ferramentas Utilizadas
---
- Java: Linguagem de programação utilizada.
- Visual Studio Code: IDE para desenvolvimento e execução do projeto.
- Terminal Linux: Para compilar e executar o código.

---
### 📦 Próximos Passos
---
- Adicionar testes unitários para validar as funcionalidades.
- Implementar uma interface gráfica para simular o uso do iPhone.
- Expandir as funcionalidades, como adicionar um sistema de mensagens ou um calendário.

---
📝 Autor
---
Desenvolvido por Guilherme como parte do desafio da DIO.

---
📄 Licença
---
 Este projeto é de uso livre para fins educacionais.


 ### Diagrma do projeto

```mermaid
classDiagram
    class ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica()
    }

    class AparelhoTelefonico {
        +ligar()
        +atender()
        +iniciarCorreioVoz()
    }

    class NavegadorInternet {
        +exibirPagina()
        +adicionarNovaAba()
        +atualizarPagina()
    }

    class iPhone {
        +tocar()
        +pausar()
        +selecionarMusica()
        +ligar()
        +atender()
        +iniciarCorreioVoz()
        +exibirPagina()
        +adicionarNovaAba()
        +atualizarPagina()
    }

    iPhone ..|> ReprodutorMusical
    iPhone ..|> AparelhoTelefonico
    iPhone ..|> NavegadorInternet
