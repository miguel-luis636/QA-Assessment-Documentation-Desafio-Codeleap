# 🐞 Bugs Documentados

---

## 🐞 Bug 1 — Login (Idioma e inconsistência de campos)

**Descrição:**
Mensagens de erro dos inputs dos formulários estão em inglês, mesmo com a aplicação voltada para português. Além disso, o campo de email aparece como "Email Address" ao invés de "Email".

**Passos para reprodução e evidência:**

1. Acessar a tela de login
2. Inserir dados inválidos nos campos
3. Observar mensagens de erro exibidas
4. Verificar o label do campo de email

Evidência: https://drive.google.com/file/d/1kGa1B7an1SzZDveFKTLQjDKxj6Id32LG/view?usp=sharing


**Resultado esperado:**

* Mensagens de erro em português
* Campo identificado como "Email"

**Resultado atual:**

* Mensagens exibidas em inglês
* Campo exibido como "Email Address"

**Severidade / Gravidade:** Média

**Possível Causa Raiz:**
Falta de padronização de internacionalização (i18n) ou uso de componentes padrão não traduzidos


---

## 🐞 Bug 2 — Login (Senha, botão e feedback)

**Descrição:**
Senha exposta sem opção de ocultar, botão de login com texto ilegível, ação de login não funciona corretamente e não há feedback de erro. Input de senha não possui limite de caracteres.

**Passos para reprodução e evidência:**

1. Acessar tela de login
2. Inserir senha no campo
3. Observar ausência de botão de ocultar senha
4. Clicar no botão de login
5. Inserir credenciais inválidas
6. Observar ausência de feedback

Evidência: https://drive.google.com/file/d/1GoSU5A3ur1giHH5-GX1RKfs39VSlf7_A/view?usp=sharing

**Resultado esperado:**

* Campo de senha com opção de ocultar/mostrar
* Botão legível e funcional
* Feedback de erro ao falhar login
* Limite de caracteres no campo

**Resultado atual:**

* Senha visível
* Botão ilegível ou não funcional
* Nenhum feedback de erro
* Sem limite de caracteres

**Severidade / Gravidade:** Alta

**Possível Causa Raiz:**
Falta de implementação de validações e ausência de tratamento de resposta da API no frontend

---

## 🐞 Bug 3 — Recuperação de senha

**Descrição:**
Ausência de feedback visual ao solicitar recuperação, não informa tempo estimado, aceita e-mails inválidos e não envia e-mail.

**Passos para reprodução e evidência:**

1. Acessar recuperação de senha
2. Inserir e-mail qualquer
3. Clicar em enviar/reenviar
4. Verificar ausência de retorno

Evidência: https://drive.google.com/file/d/1go5Jd-zayVI2k1nPkWuKYgIB0mujY8gf/view?usp=sharing

**Resultado esperado:**

* Feedback visual claro (sucesso/erro)
* Validação de e-mail
* Indicação de tempo estimado
* Envio de e-mail

**Resultado atual:**

* Sem feedback adequado
* Aceita e-mails inválidos
* Nenhuma confirmação de envio
* E-mail não é enviado

**Severidade / Gravidade:** Alta

**Possível Causa Raiz:**
Fluxo não integrado com backend ou ausência de tratamento de resposta

---

## 🐞 Bug 4 — Performance

**Descrição:**
Demora perceptível na criação de conta e outras ações.

**Passos para reprodução e evidência:**

1. Criar uma conta
2. Realizar ações como atualizar dados
3. Observar tempo de resposta

**Resultado esperado:**
Resposta rápida e fluida

**Resultado atual:**
Atraso perceptível nas ações

**Severidade / Gravidade:** Média

**Possível Causa Raiz:**
Baixa otimização de requisições ou falta de feedback durante loading

---

## 🐞 Bug 5 — Toast de notificação

**Descrição:**
Notificações exibidas em inglês.

**Passos para reprodução e evidência:**

1. Executar ação que gere notificação
2. Observar idioma

Evidência: https://drive.google.com/file/d/1t_XCYL4rHmyW3QvFB9e1kdL4FQLU8Gyc/view?usp=sharing

**Resultado esperado:**
Notificações em português

**Resultado atual:**
Notificações em inglês

**Severidade / Gravidade:** Baixa

**Possível Causa Raiz:**
Falta de tradução no sistema de notificações

---

## 🐞 Bug 6 — Slide inicial pós cadastro

**Descrição:**
Textos em inglês e uso de "lorem ipsum".

**Passos para reprodução e evidência:**

1. Criar conta
2. Observar tela inicial

Evidência: https://drive.google.com/file/d/12xaF6zxGVJ2l-I-hYSELrSN_BM8DyzYd/view?usp=sharing

**Resultado esperado:**
Conteúdo real e traduzido

**Resultado atual:**
Texto em inglês e placeholder

**Severidade / Gravidade:** Média

**Possível Causa Raiz:**
Conteúdo não finalizado (mock não substituído)

---

## 🐞 Bug 7 — Reinício do app

**Descrição:**
App aparenta reiniciar ao aceitar notificações.

**Passos para reprodução e evidência:**

1. Aceitar notificação
2. Observar comportamento do app

**Resultado esperado:**
Continuidade da navegação

**Resultado atual:**
Reinício inesperado

**Severidade / Gravidade:** Alta

**Possível Causa Raiz:**
Reinicialização do estado global ou erro no lifecycle do app

---

## 🐞 Bug 8 — Tela principal 

**Descrição:**
Header e logo exibem "crud" ao invés da marca.

**Passos para reprodução e evidência:**

1. Acessar tela principal apos login ou cadastro

Evidência: https://drive.google.com/file/d/1bL11pPZt3g-NDLTG9LQXzQOkEQPCU6ym/view?usp=sharing

**Resultado esperado:**
Nome e identidade da aplicação


**Resultado atual:**
Texto "crud"

**Severidade / Gravidade:** Baixa

**Possível Causa Raiz:**
Placeholder não substituído

---

## 🐞 Bug 9 — Busca

**Descrição:**
Busca por nome de usuário não funciona.

**Passos para reprodução:**

1. Digitar nome de usuário
2. Realizar busca

Evidência1: https://drive.google.com/file/d/1wXAYEZwefugSOdIzJEFLeMIqoKlspgEU/view?usp=sharing
Evidência2: https://drive.google.com/file/d/14e1ko6JrOv0z7VNB4OZfJCKyPmChhOGq/view?usp=sharing

**Resultado esperado:**
Resultados correspondentes

**Resultado atual:**
Nenhum resultado

**Severidade:** Média

**Possível Causa Raiz:**
Filtro não implementado ou erro na query

---

## 🐞 Bug 10 — Posts não aparecem corretamente

**Descrição:**
Posts criados não aparecem ou não são exibidos corretamente.

**Passos:**

1. Criar post
2. Voltar ao feed

Evidência: https://drive.google.com/file/d/1QgdnzKnZ1XhA4s1GbKqrXCBYyEN8Skz2/view?usp=sharing

**Resultado esperado:**
Post visível no topo

**Resultado atual:**
Post não aparece

**Severidade:** Alta

**Possível Causa Raiz:**
Falha de sincronização com backend ou estado local

Perfeito — continuando no mesmo nível e padrão 👇

---

## 🐞 Bug 11 — Tela de mensagens (conteúdo incorreto)

**Descrição:**
Ao acessar mensagens de um post, aparece “crudPost” no topo e textos “title” e “content”, que não deveriam ser exibidos.

**Passos para reprodução e evidência:**

1. Acessar um post
2. Clicar na opção de mensagens/interação
3. Observar o topo da tela e conteúdo exibido

Evidência: https://drive.google.com/file/d/1VmQx9RGkPb7_kZIU6-_D47zPMBWISg5l/view?usp=sharing

**Resultado esperado:**

* Nome do usuário ou contexto da conversa
* Conteúdo real da mensagem

**Resultado atual:**

* Texto “crudPost” no topo
* Exibição de “title” e “content”

**Severidade / Gravidade:** Média

**Possível Causa Raiz:**
Uso de dados mockados ou variáveis não substituídas no frontend

---

## 🐞 Bug 12 — Cadastro com conta existente (erro de digitação)

**Descrição:**
Mensagem de erro apresenta falha de digitação: “e -mail” ao invés de “e-mail” ou “email”.

**Passos para reprodução:**

1. Tentar criar conta com e-mail já existente
2. Observar mensagem de erro

Evidência: https://drive.google.com/file/d/1BuRzWyH_HZOqqZWChprw1J5EwoLkVrue/view?usp=sharing

**Resultado esperado:**
Mensagem com ortografia correta

**Resultado atual:**
Erro de digitação na mensagem

**Severidade:** Baixa

**Possível Causa Raiz:**
Erro de texto hardcoded

---

## 🐞 Bug 13 — Cadastro (problemas gerais)

**Descrição:**
Senha exposta, mensagens em inglês, campo “email address” e pouco feedback visual ao criar conta.

**Passos:**

1. Acessar tela de cadastro
2. Preencher dados
3. Criar conta

Evidência: https://drive.google.com/file/d/1I582jwQV9FXxbYyu698or-XlOgOOPeJ0/view?usp=sharing

**Resultado esperado:**

* Campo de senha oculto
* Mensagens em português
* Campo “Email”
* Feedback visual claro

**Resultado atual:**

* Senha visível
* Mensagens em inglês
* Campo “Email Address”
* Pouco feedback

**Severidade:** Alta

**Possível Causa Raiz:**
Falta de padronização de UI/UX e validação

---

## 🐞 Bug 14 — Scroll de posts (carregamento inconsistente)

**Descrição:**
Ícone de carregamento aparece, mas não há novos posts nem feedback de fim de lista.

**Passos:**

1. Rolar feed até o final
2. Observar loading

Evidência: https://drive.google.com/file/d/1Gybnhr4m06E61qTMrR0RMna7eeO-gS6_/view?usp=sharing

**Resultado esperado:**

* Carregar novos posts ou
* Exibir mensagem “sem mais posts”

**Resultado atual:**
Loading sem resultado

**Severidade:** Média

**Possível Causa Raiz:**
Paginação não implementada corretamente

---

## 🐞 Bug 15 — Remoção de conta

**Descrição:**
Conta não é removida mesmo após confirmação e não há feedback de erro.

**Passos:**

1. Solicitar exclusão de conta
2. Confirmar ação

Evidência: https://drive.google.com/file/d/18h1SYtkNuzHoL-M_TZnCgIyP0I3D0jul/view?usp=sharing

**Resultado esperado:**
Conta removida + feedback

**Resultado atual:**
Nada acontece

**Severidade:** Crítica

**Possível Causa Raiz:**
Endpoint não implementado ou falha na requisição

---

## 🐞 Bug 16 — Vazamento de dados entre contas

**Descrição:**
Dados de uma conta permanecem no formulário ao criar outra conta.

**Passos:**

1. Criar conta
2. Sair/criar nova conta
3. Observar formulário

Evidência: https://drive.google.com/file/d/1eB2p8AtpSKFFIie8NhPLedi9q3R6wxfU/view?usp=sharing

**Resultado esperado:**
Campos limpos

**Resultado atual:**
Dados anteriores permanecem

**Severidade:** Crítica

**Possível Causa Raiz:**
Estado não resetado corretamente

---

## 🐞 Bug 17 — Vazamento de dados em posts

**Descrição:**
Texto de conta anterior aparece ao criar post em nova conta.

**Passos:**

1. Criar conta A
2. Criar post
3. Criar conta B

Evidência: https://drive.google.com/file/d/1IHj1jXEhOsa_RlRAfmg4D7nonuPqbHLu/view?usp=sharing

**Resultado esperado:**
Campo vazio

**Resultado atual:**
Texto antigo presente

**Severidade:** Crítica

**Possível Causa Raiz:**
Persistência indevida de estado local

---

## 🐞 Bug 18 — Mensagens desaparecem

**Descrição:**
Mensagens enviadas desaparecem após 1 segundo, aceitam mensagens vazias e não permanecem visíveis.

**Passos:**

1. Enviar mensagem
2. Observar comportamento

Evidência: https://drive.google.com/file/d/1qHdMZr2rDphhSoYcKUyQn7T_8pl993B5/view?usp=sharing

**Resultado esperado:**
Mensagem persistente e validada

**Resultado atual:**
Mensagem some e aceita vazio

**Severidade:** Alta

**Possível Causa Raiz:**
Falha de sincronização com backend ou validação inexistente

---

## 🐞 Bug 19 — Atualização de perfil

**Descrição:**
Nome e sobrenome não são atualizados após edição.

**Passos:**

1. Editar perfil
2. Salvar

Evidência: https://drive.google.com/file/d/1TucBB-oqTCvoKEDU5NVVFS08qOsbXNFN/view?usp=sharing

**Resultado esperado:**
Dados atualizados

**Resultado atual:**
Dados antigos permanecem

**Severidade:** Alta

**Possível Causa Raiz:**
Falha no envio ou persistência dos dados

---

## 🐞 Bug 20 — Travamento ao iniciar app

**Descrição:**
App fica preso na tela de logo ao reiniciar.

**Passos:**

1. Fechar app
2. Abrir novamente

Evidência: https://drive.google.com/file/d/18c7_YdzOnLIyxIHHh8dZeXAA3ASQnapA/view?usp=sharing

**Resultado esperado:**
Carregamento normal

**Resultado atual:**
Tela de loading infinita

**Severidade:** Crítica

**Possível Causa Raiz:**
Erro no fluxo inicial ou carregamento de sessão

---

## 🐞 Bug 21 — Inputs sem limite de caracteres

**Descrição:**
Campos aceitam entrada ilimitada de caracteres.

**Passos:**

1. Inserir texto longo em inputs

Evidência: https://drive.google.com/file/d/1j4bAiQBOCkPsE8rXpTK8lO8UG23-UbTj/view?usp=sharing

**Resultado esperado:**
Limite definido

**Resultado atual:**
Sem limite

**Severidade:** Média

**Possível Causa Raiz:**
Validação ausente

---

## 🐞 Bug 22 — Erro de integridade de dados no cadastro

**Descrição:**
Conta criada com dados inválidos (“undefined undefined”) e sem posts.

**Passos:**

1. Criar conta com falha
2. Acessar sistema

Evidência: https://drive.google.com/file/d/1AYsbZ4xCZCsny-hWcea_JbkAUNbguPpV/view?usp=sharing

**Resultado esperado:**
Cadastro bloqueado ou dados válidos

**Resultado atual:**
Conta criada com dados inválidos

**Severidade:** Crítica

**Possível Causa Raiz:**
Falha de validação no backend e frontend
