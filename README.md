<h1 align="center">Erlon Matheus</h1>

<p align="center">
  <b>Desenvolvedor Back-end Júnior</b> · Java · PHP/Laravel · Node.js/TypeScript · PostgreSQL<br>
  Olinda – PE · disponível para trabalho remoto
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/erlon-matheus/"><img src="https://img.shields.io/badge/LinkedIn-erlon--matheus-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:erlonmtdev@gmail.com"><img src="https://img.shields.io/badge/E--mail-erlonmtdev%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="E-mail"></a>
</p>

---

Sou estudante de **Análise e Desenvolvimento de Sistemas** na UNINASSAU (conclusão prevista para o 1º semestre de 2027) e busco minha primeira oportunidade como **desenvolvedor back-end ou full stack júnior**.

Gosto de colocar as regras importantes no lugar certo. No Mural de Enquetes, o voto duplicado é barrado por uma restrição única no PostgreSQL. Na plataforma de agendamentos, dois horários não conseguem se sobrepor porque o próprio banco impede isso com uma *exclusion constraint*. Antes de escrever código, costumo documentar os requisitos e o contrato da API.

## Em andamento

- **Document Comparator**: implementando os endpoints da API em Java 21 e Spring Boot, com JPA, Flyway e testes de integração.
- **Appointment Platform**: próximos passos são isolamento entre empresas com RLS no PostgreSQL, autenticação e mais testes automatizados.

## Projetos

### [Document Comparator](https://github.com/erlonmt/document-comparator)
`Java 21` `Spring Boot` `Spring Data JPA` `Flyway` `PostgreSQL` `Docker Compose` · *em desenvolvimento*

Compara orçamentos de fornecedores: a IA sugere os dados extraídos de PDFs, o comprador revisa e o sistema indica a proposta de menor custo.

- API REST versionada (`/api/v1`) organizada em camadas: API, aplicação, domínio e persistência
- Migrations versionadas com Flyway e teste de integração com `@SpringBootTest` e relógio injetado
- Requisitos, modelo de domínio, estados de revisão, contrato da API e 36 cenários de aceitação documentados antes do código

### [Appointment Platform](https://github.com/erlonmt/appointment-platform)
`TypeScript` `Next.js` `React` `PostgreSQL` `Docker` · *em desenvolvimento*

SaaS multiempresa de agendamentos: fluxo de reserva, disponibilidade por profissional e prevenção de horários sobrepostos.

- Conflito de horários impedido no banco com *exclusion constraint* (GiST + `tstzrange`) e constraints `CHECK`
- Rotas de API para disponibilidade, profissionais e criação de reservas, com validação e códigos de erro padronizados
- Reservas com persistência transacional, testes da API e testes SQL de sobreposição

### [Mural de Enquetes](https://github.com/erlonmt/mural-enquetes)
`Laravel 11` `PHP` `React` `Node.js` `WebSocket` `PostgreSQL` `Docker`

Aplicação full stack para criar enquetes e votar, com resultados em tempo real e encerramento automático no prazo definido. Começou como teste prático de um processo seletivo.

- API REST com autenticação por token (Laravel Sanctum) e validação centralizada em FormRequest
- Voto duplicado impedido por restrição única no PostgreSQL
- Resultados em tempo real via WebSocket em Node.js; se a transmissão falhar, o voto já salvo é mantido
- Testes com PHPUnit e ambiente completo em Docker Compose

### Projetos acadêmicos

| Projeto | O que faz | Stack |
|---|---|---|
| [MobileTickets](https://github.com/erlonmt/MobileTicketsIonic) | App de emissão, chamada e relatórios de senhas para filas de laboratório, com regras de prioridade e numeração por expediente (em equipe) | Ionic, Angular, TypeScript |
| [Teleagendamento UPE](https://github.com/erlonmt/projeto_back_framework) | Agendamento de consultas que bloqueia conflitos de especialidade, data e horário. Começou como app de terminal e virou aplicação web | Python, Django, SQLite |

## Como eu trabalho

- **A regra crítica fica no banco**: restrições únicas, de exclusão e `CHECK`, não só validação no código.
- **Documentação antes da implementação**: requisitos, modelo de domínio e contrato da API.
- **Testes nos casos que mais quebram**: voto duplicado, prazo encerrado, horários sobrepostos.
- **Ambiente reproduzível**: Docker Compose e README com instalação, execução e testes.

## Tecnologias

| Área | Tecnologias |
|---|---|
| Back-end | Java 21, Spring Boot, JPA, Flyway, Maven · PHP, Laravel · Node.js, TypeScript · Python, Django |
| Banco de dados | PostgreSQL, MySQL, SQLite, modelagem relacional, migrations, constraints e transações |
| Front-end | React, Next.js, Angular, Ionic, JavaScript, HTML, CSS |
| Testes e ferramentas | JUnit 5, PHPUnit, Docker, Docker Compose, Git, GitHub, Linux |

Inglês intermediário, com leitura de documentação técnica.

---

<p align="center">Aberto a vagas de <b>Desenvolvedor Back-end Júnior</b> e <b>Full Stack Júnior</b> (remoto).<br>
<a href="https://www.linkedin.com/in/erlon-matheus/">LinkedIn</a> · <a href="mailto:erlonmtdev@gmail.com">erlonmtdev@gmail.com</a></p>
