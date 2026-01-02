# Requisitos do projeto - Game Reviews Platform

## 1. Visão geral

Uma plataforma web onde utilizadores podem:
- Criar contas
- Publicar reviews de jogos
- Ver e interagir com reviews de outros
- Gerir o seu perfil

## 2. Utilizadores

### 2.1 Tipos de Utilizadores
 - **Visitante** (não autenticado): Pode ver jogos e reviews
 - **Utilizador Registado**: Pode criar reviews, editar as suas, ver perfis
 - *Futuro: Admin/Moderador*

 ### 2.2 Usar Stories

 **Como visitante:**
 - Posso ver listas de jogos
 - Posso ver reviews de um jogo
 - Posso ver perfil público de reviewers
 - Posso registar-me

 **Como utilizador registado:**
 - Posso fazer login/logout
 - Posso criar uma review de um jogo
 - Posso editar/apagar as minhas reviews
 - Posso dar rating (1-5 ou 1-10, a definir)
 - Posso ver o meu perfil
 - Posso editar informações do meu perfil

 ### 3.Funcionalidades Detalhadas

 ### 3.1 Autenticação
 - Registo com email, username, password
 - Login com username/email e password
 - Logout
 - Validação: email único, username único, password mínimo 8 caracteres

 ### 3.2 Jogos
 - Lista paginada de jogos
 - Pesquisa por nome
 - Detalhes: título, descrição, género, ano, imagem, rating médio
 - *Decisão pendente: Quem pode adicionar Jogos? API externa? Manual?*


### 3.3 Reviews
- Criar review: texto (min 50 caracteres), rating
- Editar própria review
- Apagar própria review
- Ver todas reviews de um jogo
- Ver todas reviews de um user
- Regra: 1 review por user por jogo

## 4. Regras de Negócio
1. User só pode ter 1 review por jogo
2. User só pode editar/apagar as suas próprias reviews
3. Reviews não podem ser vazias ou muito curtas
4. Rating deve estar entre 1-10
5. Username e email devem ser unicos

## 5. Requisitos Técnicos

### 5.1 Performance
- Página deve carregar em <3 segundos
-*A definir após testes*

### 5.2 Segurança
- Password devem ser hasheadas (Bcrypt ou similar)
- Proteção contra SQL Injection
- Validação de inputs no backend
- HTTPS em produção

### 5.3 Compatibilidade
- Desktop: Chrome, Firefox, Safari (últimas 2 versões)
- Mobile: Design responsivo
- *A testar após desenvolvimento*

## 6. Fora do Scope (MVP)

Estas funcionalidades NÃO estarão na versão inicial:
- Comentários em reviews
- Likes/upvotes
- Sistema de followers
- Notificações
- Reviews de outros tipos de arte
- Chat/mensagens
- API pública

## 7. Questões em aberto

- [ ] Rating:1-5 estrelas ou 1-10 numérico?
- [ ] Quem pode adicionar novos jogos?
- [ ] Usar API externa para info de jogos (IGDB, RAWG)
- [ ] Permitir múltiplas reviews do mesmo jogo (se user mudar de opinião)?