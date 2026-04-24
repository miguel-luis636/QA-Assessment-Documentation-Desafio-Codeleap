# 🧪 Resultado dos Testes Exploratórios

## 🔍 Funcionalidades Testadas

Durante a execução dos testes exploratórios, foram avaliadas as principais funcionalidades da aplicação, com foco nos fluxos críticos do usuário:

* Login e autenticação
* Cadastro de usuário
* Recuperação de senha
* Social Feed (criação, visualização e interação com posts)
* Chat (envio e visualização de mensagens)
* Perfil (edição de dados do usuário)
* Navegação geral e comportamento da interface

---

## 🧠 Abordagem Utilizada

Foi utilizada a abordagem de **testes exploratórios**, onde aprendizado, criação e execução dos testes ocorrem simultaneamente, permitindo identificar falhas de forma dinâmica e eficiente.

Essa abordagem foi escolhida por ser mais adequada para:

* Descoberta rápida de bugs
* Identificação de problemas de usabilidade
* Exploração de comportamentos inesperados

Além disso, foram aplicadas heurísticas como:

* Testes de inputs inválidos
* Análise de consistência visual
* Validação de feedback ao usuário
* Testes de navegação e fluxo
* Exploração de estados da aplicação

---

## 🐞 Total de Bugs Encontrados

* **Total:** 22 bugs
* **Críticos:** 6
* **Altos:** 7
* **Médios:** 6
* **Baixos:** 3

---

## 🚨 Priorização de Correção

A priorização foi definida com base no impacto ao usuário e no risco para a aplicação:

### 🔴 Alta Prioridade (Críticos e Altos)

* Falha na criação e exibição de posts
* Remoção de conta não funcional
* Travamento do app na inicialização
* Vazamento de dados entre contas
* Mensagens desaparecendo no chat
* Falhas no login (sem feedback / não funcional)
* Erro de integridade de dados no cadastro

👉 Esses problemas **quebram funcionalidades principais do app**

---

### 🟠 Média Prioridade

* Problemas de UX (feedback visual ausente)
* Inconsistências de idioma (inglês/português)
* Busca não funcional
* Scroll sem retorno adequado

---

### 🟢 Baixa Prioridade

* Erros de texto (typos)
* Problemas de branding
* Conteúdos placeholder (lorem ipsum)

---

## 📊 Conclusão

A aplicação apresenta diversos problemas relevantes, principalmente em fluxos críticos como autenticação, criação de conteúdo e persistência de dados, impactando diretamente a experiência do usuário.

A utilização de testes exploratórios permitiu identificar rapidamente falhas importantes que poderiam não ser capturadas em testes mais estruturados, especialmente relacionadas a usabilidade, estados inconsistentes e comportamento inesperado do sistema.

---

## ⚡ Considerações sobre a abordagem

Como esta atividade se trata de um **assessment com tempo limitado (20 min ~ 1h)**, a abordagem adotada foi propositalmente mais direta e focada em:

* Identificação rápida de falhas críticas
* Cobertura dos principais fluxos
* Documentação objetiva dos problemas

Caso fosse solicitado um nível maior de detalhamento (como plano de testes completo, cenários formais e maior profundidade técnica), a abordagem seguiria um modelo mais estruturado, semelhante ao utilizado neste projeto:

[https://github.com/miguel-luis636/DESAFIO-QA-BEEDOO-2026](https://github.com/miguel-luis636/DESAFIO-QA-BEEDOO-2026)
