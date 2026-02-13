# 🌸 Portaria TechZone

Sistema web simples e elegante de **controle de acesso**, desenvolvido com **HTML5, CSS3 e JavaScript puro (Vanilla JS)**.

A aplicação simula uma portaria digital que valida o acesso de usuários com base no **nome cadastrado** e no **horário permitido**, oferecendo feedback visual dinâmico e intuitivo.

---

## 📌 Sobre o Projeto

O **Portaria TechZone** é uma aplicação front-end que realiza:

- ✔️ Verificação de usuário autorizado  
- ✔️ Validação de horário (0–23)  
- ✔️ Restrição de acesso após as 22h  
- ✔️ Exibição dinâmica de mensagens de sucesso ou erro  

O sistema foi desenvolvido com foco em:

- Organização de código  
- Clareza na lógica  
- Interface moderna e responsiva  
- Boas práticas de desenvolvimento  

---

## 🖥️ Tecnologias Utilizadas

- **HTML5** → Estrutura da aplicação  
- **CSS3** → Estilização com gradiente, animações e efeitos visuais  
- **JavaScript (Vanilla JS)** → Lógica de validação e manipulação do DOM  

---

## 🎨 Interface e Experiência do Usuário

A interface foi projetada com:

- 🎀 Layout centralizado
- 🌈 Fundo com gradiente moderno
- ✨ Animação de entrada suave
- 💡 Feedback visual com cores distintas:
  - Verde → Acesso permitido
  - Vermelho → Acesso negado
- 📱 Design adaptável a diferentes telas

---

## ⚙️ Funcionalidades

### 🔎 1. Validação de Horário
O sistema verifica se o valor informado está entre **0 e 23**.

Se inválido:
⛔ Horário inválido. Digite entre 0 e 23.

---

### 👤 2. Verificação de Usuário
A aplicação consulta um array interno contendo os nomes autorizados:

```javascript
let autorizados = ["Ana", "Gaby", "Paulo", "Raul"];
## ⏰ 3. Regra de Horário Limite

- Usuários cadastrados podem acessar até **21h59**
- A partir das **22h**, o acesso é bloqueado

---

## 🚦 Regras de Negócio

| Condição | Resultado |
|----------|-----------|
| Horário menor que 0 ou maior que 23 | ❌ Acesso Negado |
| Usuário não cadastrado | ❌ Acesso Negado |
| Usuário cadastrado após 22h | ❌ Acesso Negado |
| Usuário cadastrado antes das 22h | ✅ Acesso Permitido |

---

## 🧠 Conceitos Aplicados

Durante o desenvolvimento, foram trabalhados os seguintes conceitos:

- Manipulação do DOM (`getElementById`)
- Estruturas condicionais (`if`, `else if`, `else`)
- Arrays e método `.includes()`
- Conversão de tipos (`Number()`)
- Validação com `isNaN()`
- Eventos com `onclick`
- Animações com `@keyframes`
- Estilização com `box-shadow`, `transition` e `linear-gradient`
