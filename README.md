# Sistema de Eventos em Java (Console)

Este projeto implementa um sistema de cadastro e notificação de eventos em Java, seguindo o paradigma de **Programação Orientada a Objetos (POO)**. O sistema roda em console e salva os eventos em um arquivo de persistência (`events.data`).

---

## Funcionalidades

- Cadastro de usuário com **nome, e-mail e cidade**.
- Cadastro de eventos com **nome, endereço, categoria, horário e descrição**.
- Categorias pré-definidas: **FESTA, ESPORTE, SHOW, TEATRO, PALESTRA, FEIRA, OUTROS**.
- Listagem de eventos:
  - Todos os eventos (ordenados pelo horário mais próximo)
  - Próximos eventos
  - Eventos passados
  - Eventos ocorrendo agora
- Confirmação de participação em eventos e cancelamento.
- Persistência de eventos em arquivo `events.data`.
- Indicação de eventos que estão ocorrendo no momento ou já ocorreram.
- Ordenação por horário usando `java.time.LocalDateTime`.

---

## Estrutura de Classes

- `User`: informações do usuário (nome, e-mail, cidade, eventos confirmados).  
- `Event`: informações do evento (nome, endereço, categoria, horário, descrição).  
- `EventService`: regras de negócio, listagem de eventos e manipulação de participações.  
- `EventRepository`: persistência em arquivo (`events.data`) e leitura na inicialização.  
- `App`: interface de console e controlador do fluxo do sistema.  
- `Category`: enumeração das categorias de eventos.

---

## Como Executar

1. Certifique-se de ter **JDK 11 ou superior** instalado.
2. Salve todos os arquivos do projeto em uma pasta (`Main.java`, `events.data` e opcionalmente `sistema_eventos_java.pptx`).
3. Abra o terminal na pasta do projeto.
4. Compile o código:
   ```bash
   javac Main.java
