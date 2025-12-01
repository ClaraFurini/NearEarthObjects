# NASA NEO Fullstack

Aplicação fullstack para gerenciamento de Objetos Próximos à Terra (NEOs) com stack React, Node.js/Express, MongoDB, Redis e Nginx como proxy reverso com HTTPS.

# NASA NEO Fullstack

Aplicação fullstack para gerenciamento de Objetos Próximos à Terra (NEOs).  
Permite login, busca e inserção de objetos usando React no frontend, Node.js/Express no backend e MongoDB/Redis no armazenamento e cache.  
Todo o tráfego passa por Nginx com HTTPS habilitado via certificado self-signed.



## Tecnologias
- Frontend: React (SPA)
- Backend: Node.js + Express
- Banco: MongoDB
- Cache: Redis
- Proxy/HTTPS: Nginx
- Containers: Docker Compose
- Autenticação: JWT + bcryptjs


## Usuário padrão
O backend cria automaticamente:


- Senha: `123`

As rotas de NEOs exigem um token JWT obtido via `POST /api/login`.
Para gerar certificados HTTPS, execute:
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout nginx/ssl/server.key -out nginx/ssl/server.crt
email: admin@example.com
senha: 123
