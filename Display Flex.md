# Guia Completo de Flexbox

O Flexbox (\`display: flex\`) é uma ferramenta essencial no CSS para criar layouts modernos e responsivos. Este guia cobre as propriedades mais usadas e suas aplicações práticas.

---

## 1. `display: flex`
Ativa o Flexbox no contêiner e transforma seus filhos em itens flexíveis.

### Valores:
- `flex`: Ativa o modelo flexível.
- `inline-flex`: Ativa o modelo flexível, mas o contêiner é exibido como um elemento inline.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  background-color: #f4f4f4;
  padding: 20px;
  gap: 10px;
}

.box {
  background-color: #3498db;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

## 2. `flex-direction`
Controla a direção dos itens flexíveis no contêiner.

### Valores:
- `row` (padrão): Alinha os itens horizontalmente.
- `row-reverse`: Alinha horizontalmente na direção inversa.
- `column`: Alinha os itens verticalmente.
- `column-reverse`: Alinha verticalmente na direção inversa.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  flex-direction: column;
  background-color: #f4f4f4;
  padding: 20px;
  gap: 10px;
}

.box {
  background-color: #e74c3c;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

## 3. `justify-content`
Alinha os itens ao longo do eixo principal.

### Valores:
- `flex-start` (padrão): Alinha os itens no início.
- `center`: Centraliza os itens.
- `flex-end`: Alinha os itens no final.
- `space-between`: Espaço igual entre os itens.
- `space-around`: Espaço ao redor dos itens.
- `space-evenly`: Espaço igual entre e fora dos itens.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  justify-content: space-between;
  background-color: #f4f4f4;
  padding: 20px;
}

.box {
  background-color: #2ecc71;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

## 4. `align-items`
Alinha os itens no eixo cruzado (perpendicular ao eixo principal).

### Valores:
- `stretch` (padrão): Itens se esticam para preencher o contêiner.
- `flex-start`: Alinha os itens no início.
- `center`: Centraliza os itens.
- `flex-end`: Alinha os itens no final.
- `baseline`: Alinha os itens pela linha de base do texto.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box" style="height: 50px;">Box 1</div>
  <div class="box" style="height: 100px;">Box 2</div>
  <div class="box" style="height: 75px;">Box 3</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  align-items: center;
  background-color: #f4f4f4;
  padding: 20px;
}

.box {
  background-color: #9b59b6;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

## 5. `flex-wrap`
Controla se os itens devem quebrar para outra linha quando não couberem.

### Valores:
- `nowrap` (padrão): Todos os itens permanecem em uma única linha.
- `wrap`: Os itens quebram para outra linha.
- `wrap-reverse`: Os itens quebram para outra linha na direção inversa.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
  <div class="box">Box 4</div>
  <div class="box">Box 5</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  flex-wrap: wrap;
  background-color: #f4f4f4;
  padding: 20px;
  gap: 10px;
}

.box {
  background-color: #f39c12;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
  width: 100px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

## 6. `align-content`
Controla o alinhamento de **múltiplas linhas** no eixo cruzado (usado com `flex-wrap`).

### Valores:
- `flex-start`: Alinha as linhas no início.
- `center`: Centraliza as linhas.
- `flex-end`: Alinha as linhas no final.
- `space-between`: Espaço igual entre as linhas.
- `space-around`: Espaço ao redor das linhas.
- `stretch` (padrão): Linhas se esticam para preencher o contêiner.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
  <div class="box">Box 4</div>
  <div class="box">Box 5</div>
  <div class="box">Box 6</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  flex-wrap: wrap;
  align-content: space-between;
  background-color: #f4f4f4;
  padding: 20px;
  gap: 10px;
  height: 300px;
}

.box {
  background-color: #34495e;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
  width: 100px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

## 7. `gap`
Define o espaçamento entre os itens flexíveis, substituindo margens individuais.

### Valores:
- `gap`: Define o espaçamento em ambas as direções (horizontal e vertical).
- `row-gap`: Define o espaçamento vertical.
- `column-gap`: Define o espaçamento horizontal.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  gap: 20px;
  background-color: #f4f4f4;
  padding: 20px;
}

.box {
  background-color: #1abc9c;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

## 8. `flex`
Define como um item flexível cresce, encolhe ou ocupa espaço disponível.

Formato: `flex: grow shrink basis`.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box" style="flex: 1 0 200px;">Box 1</div>
  <div class="box" style="flex: 2 1 100px;">Box 2</div>
  <div class="box" style="flex: 0 1 auto;">Box 3</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  gap: 10px;
  background-color: #f4f4f4;
  padding: 20px;
}

.box {
  background-color: #e67e22;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

## 9. `order`
Controla a ordem de exibição dos itens, independentemente da ordem no HTML.

### Valores:
- Qualquer número inteiro: Define a posição relativa dos itens. Menores valores aparecem primeiro.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box" style="order: 2;">Box 1</div>
  <div class="box" style="order: 1;">Box 2</div>
  <div class="box" style="order: 3;">Box 3</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  background-color: #f4f4f4;
  padding: 20px;
  gap: 10px;
}

.box {
  background-color: #8e44ad;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

## 10. `align-self`
Ajusta o alinhamento individual de um item no eixo cruzado, ignorando `align-items`.

### Valores:
- `auto` (padrão): Segue o valor de `align-items`.
- `flex-start`: Alinha no início.
- `center`: Centraliza no eixo cruzado.
- `flex-end`: Alinha no final.
- `baseline`: Alinha pela linha de base.
- `stretch`: Estica o item para preencher o contêiner.

### Exemplo de HTML:
```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box" style="align-self: flex-end;">Box 2</div>
  <div class="box">Box 3</div>
</div>
```

### Exemplo de CSS:
```css
.container {
  display: flex;
  align-items: center;
  background-color: #f4f4f4;
  padding: 20px;
}

.box {
  background-color: #c0392b;
  color: white;
  padding: 20px;
  text-align: center;
  border-radius: 5px;
}
```

**[Espaço para imagem do exemplo sendo aplicado]**

---

Com este guia, você terá controle total sobre layouts flexíveis e responsivos com Flexbox! 🚀
