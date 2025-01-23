# Flexbox: As 10 Propriedades Mais Usadas

O Flexbox (\`display: flex\`) é uma ferramenta poderosa para criar layouts responsivos e flexíveis. Este guia cobre as 10 propriedades mais usadas com exemplos e explicações para ajudá-lo a dominar o Flexbox.

## 1. `display: flex`
Ativa o Flexbox no contêiner e transforma seus filhos em itens flexíveis.

```css
.container {
  display: flex;
}
```

---

## 2. `flex-direction`
Controla a direção dos itens flexíveis no contêiner.

Valores comuns:
- `row` (padrão): Alinha os itens horizontalmente.
- `row-reverse`: Alinha horizontalmente na direção inversa.
- `column`: Alinha os itens verticalmente.
- `column-reverse`: Alinha verticalmente na direção inversa.

```css
.container {
  flex-direction: row;
}
```

---

## 3. `justify-content`
Alinha os itens ao longo do eixo principal.

Valores comuns:
- `flex-start`: Alinha os itens no início.
- `center`: Centraliza os itens.
- `flex-end`: Alinha os itens no final.
- `space-between`: Espaço igual entre os itens.
- `space-around`: Espaço ao redor dos itens.
- `space-evenly`: Espaço igual entre e fora dos itens.

```css
.container {
  justify-content: center;
}
```

---

## 4. `align-items`
Alinha os itens no eixo cruzado (perpendicular ao eixo principal).

Valores comuns:
- `stretch` (padrão): Itens se esticam para preencher o contêiner.
- `flex-start`: Alinha os itens no início.
- `center`: Centraliza os itens.
- `flex-end`: Alinha os itens no final.
- `baseline`: Alinha os itens pela linha de base do texto.

```css
.container {
  align-items: center;
}
```

---

## 5. `flex-wrap`
Controla se os itens devem quebrar para outra linha quando não couberem.

Valores comuns:
- `nowrap` (padrão): Todos os itens permanecem em uma única linha.
- `wrap`: Os itens quebram para outra linha.
- `wrap-reverse`: Os itens quebram para outra linha na direção inversa.

```css
.container {
  flex-wrap: wrap;
}
```

---

## 6. `align-content`
Controla o alinhamento de **múltiplas linhas** no eixo cruzado (usado com `flex-wrap`).

Valores comuns:
- `flex-start`: Alinha as linhas no início.
- `center`: Centraliza as linhas.
- `flex-end`: Alinha as linhas no final.
- `space-between`: Espaço igual entre as linhas.
- `space-around`: Espaço ao redor das linhas.
- `stretch` (padrão): Linhas se esticam para preencher o contêiner.

```css
.container {
  align-content: space-between;
}
```

---

## 7. `flex`
Define como um item flexível cresce, encolhe ou ocupa espaço disponível.

Formato: `flex: grow shrink basis`.

Valores comuns:
- `flex: 1`: O item cresce proporcionalmente para preencher o espaço.
- `flex: 0 1 auto`: Comportamento padrão.
- `flex: none`: Desabilita comportamento flexível.

```css
.item {
  flex: 1;
}
```

---

## 8. `order`
Controla a ordem de exibição dos itens, independentemente da ordem no HTML.

```css
.item:first-child {
  order: 2;
}
.item:last-child {
  order: 1;
}
```

---

## 9. `gap`
Define o espaçamento entre os itens flexíveis.

```css
.container {
  display: flex;
  gap: 16px;
}
```

---

## 10. `align-self`
Ajusta o alinhamento individual de um item no eixo cruzado, ignorando `align-items`.

Valores comuns:
- `auto` (padrão): Segue o valor de `align-items`.
- `flex-start`, `center`, `flex-end`, `baseline`, `stretch`.

```css
.item {
  align-self: flex-end;
}
```

---

## Exemplo Completo:

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 20px;
}

.item {
  flex: 1;
  order: 2;
  align-self: center;
}
```

Com essas 10 propriedades, você pode criar layouts flexíveis e responsivos com facilidade! 🚀
