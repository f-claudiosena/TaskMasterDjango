# TaskMasterAPI com Django + React

Este projeto é uma aplicação de lista de tarefas (to-do) com backend em Django e frontend em React.

## Backend (Django)

### Configuração

1. Crie e ative um ambiente virtual:
   ```bash
   cd backend
   python3 -m venv venv
   source venv/bin/activate
   ```

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

3. Realize as migrações:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

4. (Opcional) Crie um superusuário:
   ```bash
   python manage.py createsuperuser
   ```

5. Inicie o servidor:
   ```bash
   python manage.py runserver
   ```

- Acesse a API REST em: `http://localhost:8000/api/tasks/`
- Acesse o admin do Django em: `http://localhost:8000/admin/`

## Frontend (React)

(Sua estrutura de frontend pode ser igual ao projeto anterior — só ajuste as URLs das requisições para o endpoint Django.)

1. Instale as dependências:
   ```bash
   cd client
   npm install
   ```

2. Rode o frontend:
   ```bash
   npm start
   ```

## Observações

- O CORS já está liberado para desenvolvimento (`CORS_ALLOW_ALL_ORIGINS = True`).
- Para produção, configure variáveis sensíveis e restrinja o CORS.
- O banco padrão é SQLite, mas pode ser alterado para PostgreSQL facilmente.

---