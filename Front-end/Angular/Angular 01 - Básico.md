## Property Binding
```typescript
pensamento = {
conteudo: 'Aprendendo Angular',
};
```

Utilizado em propriedades ou com **interpolação**.

```html
<input
type="textarea"
class="input"
[value]="pensamento.conteudo"
/>

<!-- Interpolação-->

<p>{{ pensamento.conteudo }}</p>
```




