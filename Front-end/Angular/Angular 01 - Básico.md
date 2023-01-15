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

## Two-way data-binding
Utilizando **[(ngModel)]**.
```html
<input
	type="textarea"
	class="input"
	[(ngModel)]="pensamento.conteudo"
/>
```

## ngFor, ngIf e ng-template.
O *ngFor* é utilzado para renderizar um conjunto de elementos *ngIf* para renderizacao condicional e o *ng-template* para ser renderizado apenas quando for chamado.
```html

<h2 *ngIf="naoExistemPensamentos">
	Ainda não há pensamentos cadastrados!
</h2>

<div *ngFor="let pensamento of listaPensamentos">
	<app-pensamento [pensamento]="pensamento"></app-pensamento>
</div>


<ng-template #semPensamentosMessage>
	<div class="ff-inter sem-pensamentos">
		<p>Ainda não há pensamentos cadastrados!</p>
	</div>

</ng-template>
```

## NgClass
Estilos condicionais, 
