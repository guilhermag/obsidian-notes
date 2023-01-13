## Property Binding

```typescript
pensamento = {
	conteudo: 'Aprendendo Angular',
};
```
Utilizado em propriedades, com a lógica **[propriedade]="valor"** ou com **interpolação**.
```html
<input
	type="textarea"
	class="input"
	[value]="pensamento.conteudo"
/>
<!-- Interpolação-->
<p>{{ pensamento.conteudo }}</p>
```
## Event Binding

Utiliza **(evento)="método()"**.
```typescript
criarPensamento() {
	alert('apertado');
}
```
Utilizado em propriedades, com a lógica **[propriedade]="valor"** ou com **interpolação**.
```html
<button (click)="criarPensamento()" class="botao">Salvar</button>
```



