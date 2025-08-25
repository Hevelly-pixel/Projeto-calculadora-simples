# 🧮 Calculadora Simples

## 🎯 Objetivo  
Desenvolver uma calculadora funcional utilizando **HTML, CSS e JavaScript**, com interface simples e amigável para praticar fundamentos de desenvolvimento web.

---

## 🛠️ Tecnologias Utilizadas  
- **HTML5** → estrutura da aplicação  
- **CSS3** → estilização e layout  
- **JavaScript (ES6)** → lógica e funcionamento das operações  

---

## 🚀 Funcionalidades  
- Realizar operações matemáticas básicas: `+`, `-`, `×`, `÷`  
- Suporte a números decimais  
- Botão de limpar (`C`)  
- Interface intuitiva e responsiva  
- Tratamento de erros simples (como expressões inválidas)  

---

## 📌 Estrutura do Código  

### 📄 index.html  
```html
<input type="text" id="display" disabled>
<div class="buttons">
  <button class="clear" onclick="clearDisplay()">C</button>
  <button onclick="appendValue('7')">7</button>
🎨 style.css
button {
  padding: 15px;
  font-size: 18px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  background: #eee;
}
button:hover {
  background: #ddd;
}
⚡ script.js
function appendValue(value) {
  display.value += value;
}
function clearDisplay() {
  display.value = "";
}
function calculate() {
  try {
    display.value = eval(display.value);
  } catch {
    display.value = "Erro";
  }
}


