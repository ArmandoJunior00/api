# 📝 API de Tarefas Simples com Spring Boot

Esta é uma API simples desenvolvida com **Java Spring Boot** que permite realizar operações básicas de CRUD em uma lista de tarefas. Os dados são armazenados temporariamente em memória (através de uma lista), o que torna essa aplicação ideal para fins educacionais e testes locais.

---

## 🚀 Tecnologias Utilizadas

- Java 17+
- Spring Boot
- Spring Web
- Jackson (para serialização JSON)

---

## 📂 Estrutura do Projeto

O projeto possui um único controller:

```
br.com.api.controller.ApiController
```

---

## 📌 Endpoints da API

### ✅ Listar Tarefas

- **Método:** `GET`
- **URL:** `/tasks`
- **Descrição:** Retorna todas as tarefas cadastradas até o momento.

📥 **Exemplo de Resposta:**
```json
["Estudar Spring", "Finalizar projeto"]
```

---

### ➕ Criar Tarefa

- **Método:** `POST`
- **URL:** `/tasks`
- **Descrição:** Adiciona uma nova tarefa à lista.

📤 **Exemplo de Requisição:**
```json
"Estudar Spring"
```

📥 **Resposta:** `200 OK` (sem conteúdo)

---

### 🗑️ Deletar Todas as Tarefas

- **Método:** `DELETE`
- **URL:** `/tasks`
- **Descrição:** Remove todas as tarefas da lista.

📥 **Resposta:** `200 OK`

---

## ⚠️ Observações

- As tarefas são armazenadas **somente em memória**, ou seja, ao reiniciar a aplicação, a lista será resetada.
- Ideal para fins didáticos ou para ser expandido com persistência em banco de dados (JPA, MongoDB, etc).

---

## 🧪 Como Executar o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/ArmandoJunior00/api
   ```
2. Abra o projeto em sua IDE favorita (IntelliJ, Eclipse, VSCode).
3. Certifique-se de ter o Java e o Maven instalados.
4. Rode a aplicação:
   ```bash
   ./mvnw spring-boot:run
   ```
5. Acesse os endpoints via Postman ou outro cliente HTTP em:
   ```
   http://localhost:8080/tasks
   ```

---

## 📫 Contato

Caso queira contribuir ou tirar dúvidas:

- Nome: Armando Junior
- Email: armaanijr00@gmail.com
- LinkedIn: https://www.linkedin.com/in/armandojunior00/

---

Feito com 💻 e ☕ por Armando Junior
