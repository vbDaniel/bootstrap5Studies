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

### Style with Bootstrap

- Como deixar uma tabela responsiva ao tamanho da tela com Bootstrap: 

Deve-se inserir toda a tabela dentro de um <div> e inserir a classe "table-responsive":
  
```HTML
   <div "table-responsive">
      <table  class="table table=striped table-bordered table hover">
          <thead>
            <tr>
              <th>Ingredients</th>
              <th>Risk</th>
              <th>Cal</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Açúcar </td>
              <td>YEs</td>
              <td>400g</td>
            </tr>
            <tr>
              <td>Mamão  </td>
              <td>No</td>
              <td>3g</td>
            </tr>
          </tbody>
      </table>
   </div>
```
Assim quando temos uma tela menor aparecerá  um barra de scroll. 

- Como deixar uma imagem responsiva ao tamanho da tela com Bootstrap:
  
  
 Só é necessário adcionar a class="image-fluid":
  
 ```HTML
    <div class="col-lg-4 col-sm-8">
        <img src="images/bethanylogo.png" alt="Logo"  class="rounded img-fluid/>
    </div>  
```
Assim a imagem irá reduzir ou almentar de acordo com o tamanho da tela.


Aplicar Padding and margin:
    
  - pb-3 : Padding bottom of 3;
                                                         
  - p-3 : Padding todos os lugares em 3;
                                                             
  - me-0: margin of right of 0;
  
  - py-5: Padding vertical of 5;                                                           

Aplicar Border:
```HTML                                                             
 <span class="border">
  ...
 </span>                                                          
```                   

## Componets 

 Basic Components:
   - Alert                 
   - Button
   - Breadcrumb                  
   - Nav & Navbar                    
   - Card                
   - Progress                  
 
 Basic Nav e Navbar 

 ```HTML                    
 <nav  class="navbar navbar-expand-lg navbar-dark fixed-top bg-dark "> // Vai setar um background escuro e fixar na tela indepentdente da rolagem.
                                                            
          <ul class="nav nav-pills bg-light">
              <li class= "nav-item">
                <a class="nav-item active" href= "index.html">Home</a> // Active mostrara em um forma visual que está ativo
              </li>   
              <li class= "nav-item">
                <a class="nav-item" href= "seasonalpies.html">Pies</a>
              </li>                                                          
              <li class= "nav-item">
                <a class="nav-item" href= "order.html">Orders</a>
              </li>                                                                                                               
          </ul>
   </nav>                     
  ```               
 
Forms creating:
                                                                                                                                                                 
                                                      
                     
                     
                     
                     
