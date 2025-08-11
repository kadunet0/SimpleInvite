# SimplyInvite

## 📌 Visão Geral

O **SimplyInvite** é uma plataforma que conecta **jovens talentos**, **gestores** e **profissionais de RH**, permitindo recrutamento, avaliação e acompanhamento por meio de **projetos, vídeos e entrevistas**.  
O sistema possui **frontend moderno** em React + Vite e **backend robusto** em Java Spring Boot, com persistência em PostgreSQL, pronto para execução local ou via Docker.

---

## 🛠️ Tecnologias

### Frontend
- React + TypeScript
- Vite
- Tailwind CSS
- shadcn-ui
- Lucide Icons
- Axios
- React Router
- React Hook Form + Zod
- Sonner (notificações)

### Backend
- Java 17 + Spring Boot 3
- Spring Data JPA
- Spring Security + JWT
- PostgreSQL
- H2 (para testes)
- Maven

### DevOps
- Docker + Docker Compose

---

## 📂 Estrutura de Pastas

simplyinvite-showcase-page/
├── backend/ # Backend Java Spring Boot
│ ├── modelos/ # Entidades JPA
│ ├── repositorios/ # Repositórios JPA
│ ├── servicos/ # Regras de negócio
│ ├── controladores/ # Controllers REST
│ ├── dtos/ # Objetos de transferência
│ └── seguranca/ # JWT e configs de segurança
├── frontend/ # Frontend React + Vite
│ ├── components/ # Componentes reutilizáveis
│ ├── pages/ # Páginas por perfil (talento, gestor, RH)
│ ├── contexts/ # Contextos (ex.: Auth)
│ ├── hooks/ # Hooks customizados
│ └── servicos/ # Serviços API
├── docker-compose.yml
└── README.md

---

## ✨ Funcionalidades

### Jovens Talentos
- Criação de perfil com dados acadêmicos e profissionais
- Envio de vídeos de apresentação e projetos
- Visualização de feedbacks
- Agendamento de entrevistas

### Gestores
- Avaliação de talentos e projetos
- Feedback detalhado
- Sistema de medalhas
- Agendamento de entrevistas

### RH
- Gestão de processos seletivos
- Avaliação preliminar de candidatos
- Acompanhamento de feedbacks
- Organização de entrevistas

---

## 🚀 Como Executar

### Usando Docker (recomendado)
```bash
git clone <URL_DO_REPOSITORIO>
cd simplyinvite-showcase-page
docker-compose up --build
Acesse:

Frontend: http://localhost

Backend: http://localhost:8080

PostgreSQL: localhost:5432 (user: postgres | pass: jonas1385)

Desenvolvimento Local
Backend

bash
Copiar
Editar
cd backend
mvnw spring-boot:run
Frontend

bash
Copiar
Editar
cd frontend
npm install
npm run dev
🔑 Credenciais de Teste
Perfil	Email	Senha
Jovem Talento	jovem@example.com	senha123
RH	rh@example.com	senha123
Gestor	gestor@example.com	senha123

⚙️ Variáveis de Ambiente
Arquivo .env:

ini
Copiar
Editar
PORT=8080
DB_HOST=postgres
DB_USER=postgres
DB_PASS=jonas1385
DB_NAME=simplyinvite
JWT_SECRET=simplyinvite_secret_key_12345
🤝 Contribuindo
Fork do repositório

Crie uma branch: git checkout -b feature/nova-feature

Commit: git commit -m "Descrição"

Push: git push origin feature/nova-feature

Abra um Pull Request

📧 Suporte
E-mail: suporte@simplyinvite.com
