
# 🎓 API Acadêmica — Backend em Spring Boot

API REST desenvolvida em Java com Spring Boot para gerenciamento acadêmico. Permite cadastrar e consultar alunos, cursos, disciplinas e turmas, além de realizar matrículas e associar disciplinas às turmas. Ideal para sistemas educacionais com estrutura modular e escalável.

## 🚀 Tecnologias utilizadas

- Java 17+
- Spring Boot
- Spring Data JPA
- Hibernate
- PostgreSQL (ou outro banco relacional)
- Maven
- Swagger (opcional para documentação)

---

## 📦 Funcionalidades da API

### Alunos
- `GET /alunos` — Lista todos os alunos
- `POST /alunos` — Cadastra um novo aluno

### Cursos
- `GET /cursos` — Lista todos os cursos
- `POST /cursos` — Cadastra um novo curso

### Disciplinas
- `GET /disciplinas` — Lista todas as disciplinas
- `POST /disciplinas` — Cadastra uma nova disciplina

### Turmas
- `GET /turmas` — Lista todas as turmas com curso, disciplinas e alunos
- `POST /turmas` — Cadastra uma nova turma
- `POST /turmas/{turmaId}/disciplinas/{disciplinaId}` — Associa uma disciplina à turma
- `POST /turmas/{turmaId}/alunos/{alunoId}` — Matricula um aluno na turma

---

## 🛠️ Como executar localmente

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/api-academica.git

# Acesse a pasta
cd api-academica

# Configure o application.properties com suas credenciais de banco

# Execute o projeto
./mvnw spring-boot:run

