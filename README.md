# api-manage-medical-appointments
API RESTful de Gerenciamento de Consultas Médicas.

- **CRUD completo:**
    -  Profissionais da saúde
    - Consultas (relacionadas a profissionais)
    -  Busca de consultas pelo ID do profissional
    
-  **Segurança obrigatória:**
    -  Sanitização e validação dos dados
    -  Proteção contra SQL Injection
    -  Implementação de CORS configurado corretamente
    -  Controle básico de autenticação (ex.: API Key, JWT ou Token simples)
    -  Logs de acesso e erros
    
-  **Tecnologias obrigatórias:**
    - Python com Django + Django REST Framework
    - Poetry (gerenciamento de dependências)
    - PostgreSQL
    - Docker (containerização)
    - GitHub Actions (para CI/CD)
-  **Testes automatizados:**
    -  Usando `APITestCase` do Django
    -  Cobertura mínima: 
      - CRUD de consultas
      - CRUD de profissionais
      - Testes de erro (ex.: requisição inválida, dados ausentes)
-  **Deploy funcional:**
    -   Ambientes separados: staging e produção (AWS)
    
-  **Pipeline CI/CD:**
    -  GitHub Actions com steps obrigatórios:
      - Lint
      - Testes
      - Build
      - Deploy
- **Documentação obrigatória:**
    - README com setup local e via Docker
    - Execução dos testes
    - Fluxo de deploy (CI/CD)
    - Justificativas técnicas das escolhas feitas
    - **Proposta de rollback funcional:**
        - Ex.: Deploy Blue/Green, Revert no GitHub Actions, Preview Deploy
-  **Features futuras:**
    - Proposta de integração com a Assas (mock, arquitetura ou real)
    - Geração de documentação da API (ex.: Swagger, Redoc, Postman)
