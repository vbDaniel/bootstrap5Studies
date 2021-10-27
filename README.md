# bootstrap5Studies
Estudos sobre a nova versão  de bootstrap5

Bootstrap 5 é um CSS frame work que auxilia com varios Building BLock:

- Layout
- Components
- Interactivity
- Style Utilities
- THeming Style

Algumas das principais  vantagens do uso são:

- Consistência 
- Lightweight
- Responsive (funciona em qualquer aparelho)
- Community (grande fórum  sobre dúvidas, bugs e outros)
- Templates
- Possui o suporte de todos os grandes browsers

## Bootstrap Grid System:

Essse sistema é usado apenas para layout é baseado em um esquema de 12 colunas e múltiplas linhas dentro de um ou mais conteiner:


Breakpoint: Adapta para diferentes formatar do grid.

![Screen Shot 2021-10-27 at 12 57 36](https://user-images.githubusercontent.com/87997848/139102899-1a79e8b8-a097-4eae-b79c-9bc6953becd7.png)

- The container:
```HTML
<div class="container"> // Pode-se usar o conceito do BreakPoint como '.container-sm'que seria um conteiner pequeno
  ...
</div>  
//or
<div class="container-fluid">
  ...
</div>  
```
- The Row and Column:

A cada row(linha) pode-se ter até 12 colunas, pois o 12 é um valor que possibilita  criar diversos conceitos.

Para se usar as colunas pode serem aplicas em `<div>` 's:

```HTML
<div class="container">
    <div class="row">
         <div class="col">
                1
         </div>  
         <div class="col-6">
                1
         </div>  
         <div class="col">
                1
         </div>  
    </div>  
</div>  
```

O tamanho de um col também  é dada pelo prefix de um breakpoint  como "col-md".

![Screen Shot 2021-10-27 at 14 08 04](https://user-images.githubusercontent.com/87997848/139113370-c0373326-2875-4014-af38-a6c029c39fe8.png)

Os prefixos como "-md"/"-xx" podem ser usados para quando a tela de um tamanhao "-sm" se organizar  no gride de uma forma se não  de outra. 

```HTML
    <div class="row">
         <div class="col-md-8 col-sm-4">
                1
         </div>   
         <div class="col-md-4 col-sm-8">
                1
         </div>  
    </div>  
```

Para deixa um vazio =>  
```HTML
<div class="col-md-4 offset-md-6">
      ...1
</div>  
```
Para organizar de outra forma usa order-n(o valor do número vai definir para onde sera movido):
```HTML
<div class="col-md-4 order-1 "> // movido para a esquerda
      ...1
</div>  
```
Para deixar um pequeno  espaço entre os elementos usa-se gutter(gx-n) n define o qual largo ou nenhum com 0:
```HTML
    <div class="row gx-4">
         <div class="col-md-2">
                1
         </div>   
         <div class="col-md-4">
                1
         </div>  
    </div>  
```




















