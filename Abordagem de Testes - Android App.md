# 📱 Template App - QA Assessment

## 📌 Sobre o Projeto

Este repositório documenta a execução de testes em uma aplicação mobile fornecida pela CodeLeap, com o objetivo de avaliar habilidades práticas em Quality Assurance, incluindo identificação de bugs, análise de usabilidade e abordagem de testes.

---

## 🧪 Abordagem de Testes

A estratégia adotada foi baseada em **testes exploratórios**, com foco na interação real do usuário com a aplicação. Esse tipo de abordagem permite identificar rapidamente falhas críticas, comportamentos inesperados e problemas de usabilidade sem a necessidade de casos de teste previamente definidos.

Durante os testes, o foco principal foi **identificar falhas que impactam diretamente o funcionamento do aplicativo**, priorizando problemas que possam comprometer a experiência do usuário ou impedir o uso das funcionalidades principais.

---

## 🎯 Priorização de Testes

A priorização foi baseada no impacto para o usuário final e no risco de falhas visíveis:

* Criação e Login de Conta
* Criação e interação com posts 
* Envio e recebimento de mensagens 
* Edição e salvamento de dados do perfil 

> “Priorizei funcionalidades críticas como criação de posts, envio de mensagens e edição de perfil, por terem maior impacto na experiência do usuário.”
> “Fluxos principais foram priorizados por representarem maior risco de falhas visíveis ao usuário final.”

---

## 🧠 Heurísticas Aplicadas

Durante a execução dos testes exploratórios, foram utilizadas heurísticas para guiar a identificação de problemas:

* **Testes de Inputs**: validação de campos com dados inválidos, vazios, longos ou com caracteres especiais
* **Consistência e Padrões**: verificação de comportamentos inconsistentes entre telas e funcionalidades
* **Feedback ao Usuário**: análise de respostas da interface após ações (ex: cliques sem retorno visual)
* **Navegação e Fluxo**: validação de transições entre telas e funcionamento do botão “voltar”
* **Estados da Aplicação**: testes considerando diferentes cenários (ex: sem internet, carregamento, ações repetidas)

Essas heurísticas ajudaram a focar não apenas em falhas funcionais, mas também em problemas de experiência do usuário (UX).

---

## 🐞 Bugs e Melhorias Encontrados

Os bugs identificados foram documentados considerando:

* Passos para reprodução
* Resultado esperado
* Resultado atual
* Severidade / Gravidade
* Possivel Causa Raiz

(Favor consultar a seção ou arquivo de bugs para mais detalhes)

---

## ⚠️ Problemas de Usabilidade e Melhorias

Além dos bugs funcionais, também foram identificados pontos de melhoria relacionados à experiência do usuário, como falta de feedback visual, inconsistências de interface e possíveis confusões na navegação.

---

## 📊 Considerações Finais

A abordagem priorizou eficiência e foco em impacto, buscando identificar rapidamente falhas críticas e problemas visíveis ao usuário final. O uso de testes exploratórios aliado a heurísticas permitiu uma análise abrangente da aplicação dentro do tempo proposto.
