# 📦 Mini Loja - Exibição de Produtos

Este é um pequeno projeto que exibe produtos em um layout responsivo utilizando **HTML, CSS e Bootstrap 5**. Os produtos possuem uma interface interativa com botões de adição e remoção de quantidade.

## 🚀 Tecnologias Utilizadas

- **HTML5**
- **CSS3**
- **Bootstrap 5**
- **JavaScript (para controle da quantidade de produtos)**

## 📌 Funcionalidades

✅ Exibição de produtos em um layout responsivo  
✅ Animação ao passar o mouse sobre os produtos  
✅ Botões "+" e "-" para ajustar a quantidade de produtos  
✅ Layout adaptável para diferentes dispositivos  

## 🎨 Estilo e Responsividade

- Os produtos têm um design moderno com sombras e efeitos ao passar o mouse.
- O layout utiliza **Bootstrap Grid**, tornando a página responsiva automaticamente.
- Os botões utilizam estilos do Bootstrap para melhor usabilidade.

## 📂 Estrutura do Projeto

```
/mini-loja
│── index.html        # Página principal com exibição dos produtos
│── css/style.css     # Estilos personalizados (opcional)
│── bg.jpeg           # Imagem de fundo dos produtos (substitua por uma imagem válida)
│── README.md         # Documentação do projeto
```

## 🛠 Como Usar

1️⃣ Clone este repositório:
```sh
git clone https://github.com/pedromael/lista-de-produtos-basico.git
```

2️⃣ Acesse a pasta do projeto:
```sh
cd mini-loja
```

3️⃣ Abra o arquivo `index.html` no navegador.

## 📜 Código de Exemplo

### **Trecho do HTML**
```html
<div class="produto">
    <p class="preco">X<span>0</span></p>
    <div class="add_prod">
        <button class="btn btn-add menos">-</button>
        <button class="btn btn-add mais">+</button>
    </div>
    <div class="descricao">
        <p class="nome h5 text-dark">Produto</p>
        <p class="descr small">Um pão com tudo, muito bom</p>
    </div>
</div>
```

### **JavaScript para Controle de Quantidade**
```js
document.querySelectorAll('.produto').forEach(produto => {
    let preco = produto.querySelector('.preco span');
    let btnMais = produto.querySelector('.mais');
    let btnMenos = produto.querySelector('.menos');
    
    let quantidade = 0;

    btnMais.addEventListener('click', () => {
        quantidade++;
        preco.textContent = quantidade;
    });

    btnMenos.addEventListener('click', () => {
        if (quantidade > 0) {
            quantidade--;
            preco.textContent = quantidade;
        }
    });
});
```

## 📌 Melhorias Futuras

🔹 Conectar com um backend para armazenar os produtos  
🔹 Implementar um sistema de carrinho de compras  
🔹 Adicionar animações e efeitos visuais aprimorados  

---

### 📢 **Contribuição**
Sinta-se à vontade para melhorar este projeto! Faça um **fork**, crie uma **branch** e envie um **pull request** 🚀.

### 📩 **Contato**
📧 Email: pedromael14@gmail.com
🐙 GitHub: [pedromael](https://github.com/pedromael)  

---

🛒 **Mini Loja - Criado para exibir produtos de forma interativa e responsiva!**  
