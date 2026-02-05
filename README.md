# 🏋️‍♂️ SIGA — Sistema Integrado de Gestão de Academia

O **SIGA** é uma solução de software robusta para a **gestão inteligente de academias**, focada na **automação de presença via hardware mobile (QR Code)**, **gestão de treinos** e **análise de dados** para apoio à tomada de decisão.

Desenvolvido por **Víctor Matheus Tavares Rafael**, estudante de **Engenharia de Software na UTFPR**.

---

## 📑 Visão Geral e Elaboração

O projeto foi concebido para resolver o gargalo de **controle de acesso** e **engajamento** em ambientes fitness.  
A elaboração seguiu o modelo de **Desenvolvimento Ágil**, com foco em **entregas incrementais** e **validação constante da arquitetura**.

---

## ⏱️ Cronograma de Desenvolvimento (Sprints)

O projeto foi dividido em um ciclo intenso de **3 semanas**:

### 🔹 Sprint 1 — Estudo e Planejamento (Fundamentação)
- Análise técnica da stack: **Angular 17 (Standalone)** e **NestJS**
- Modelagem do banco de dados relacional com **Prisma ORM**
- Definição da arquitetura de segurança (**JWT & RBAC**)
- Planejamento de **UI/UX** com foco em acessibilidade e performance mobile

### 🔹 Sprint 2 — Core Engineering (Backend & Auth)
- Implementação do servidor **NestJS** e conexão com **PostgreSQL**
- Desenvolvimento do sistema de autenticação e controle de níveis de acesso (**Admin / Aluno**)
- Criação dos **scripts de Seed** para teste de carga inicial

### 🔹 Sprint 3 — Experiência do Usuário e Integração (Frontend)
- Desenvolvimento do **leitor de QR Code** para registro de presença
- Criação de **dashboards reativos** com **RxJS** e gráficos de frequência
- Implementação da **Central de Dúvidas** e sistema de **notificações assíncronas**

---

## 🛠️ Requisitos do Sistema

### ✅ Requisitos Funcionais (RF)

| ID   | Nome                   | Descrição                                                         |
|------|------------------------|-------------------------------------------------------------------|
| RF01 | Autenticação por Nível | O sistema deve distinguir entre administradores e alunos no login |
| RF02 | Registro por QR Code   | Alunos devem registrar presença via scan de código dinâmico       |
| RF03 | Bloqueio de Acesso     | O aluno não pode visualizar o treino sem antes registrar presença |
| RF04 | Gestão de Treinos     | O Admin pode criar, editar e excluir fichas de treino (CRUD)      |
| RF05 | Central de Dúvidas    | Alunos podem enviar mensagens categorizadas ao treinador          |
| RF06 | Analytics              | Dashboard de frequência com exportação de dados para o Admin      |

### ⚙️ Requisitos Não-Funcionais (RNF)

- **Segurança:**  
  Todas as rotas da API protegidas por **JWT**; senhas criptografadas com **bcrypt**
- **Disponibilidade:**  
  Arquitetura preparada para deploy em **Cloud (AWS / Railway)**
- **Performance:**  
  Uso de **Lazy Loading** e **Standalone Components** no frontend
- **Escalabilidade:**  
  Banco preparado para crescimento do histórico de frequências sem perda de performance

---

## 🏗️ Stack Tecnológica

O SIGA utiliza uma stack moderna, focada em **produtividade** e **tipagem forte**:

- **Frontend:** Angular 17+, Angular Material, RxJS, Chart.js  
- **Backend:** NestJS, TypeScript, Passport.js  
- **Persistência:** PostgreSQL, Prisma ORM  
- **Infraestrutura:** Docker, Cloud Deployment (contexto AWS Cloud Practitioner)

---

## 📊 Métrica de Sucesso (KPI)

A eficiência do sistema é medida pela **Taxa de Ocupação Real** e pelo **tempo médio de resposta** entre o scan do QR Code e a liberação do treino:

**Frequência Relativa (%) = (Presenças Confirmadas / Alunos Matriculados) × 100**

---

## 👨‍💻 Desenvolvedor

**Víctor Matheus Tavares Rafael**  
🎓 Engenharia de Software — UTFPR  
☁️ AWS Certified Cloud Practitioner