# Sobre o Teste
## Desafio da Ampulheta

Na [Pasta print](https://github.com/devartes/desafio/tree/master/print) , foi usado somente Javascript e na [Pasta window prompt](https://github.com/devartes/desafio/tree/master/window%20prompt) , foi usado Javascript e Html.


- VS Code e [JSFiddle](https://jsfiddle.net/) me auxiliaram durante a criação do código.
- Este [site](https://www.javatpoint.com/star-program-in-c) me serviu como base para conseguir obter estes dois resultados.

## Como cheguei a este resultado?

> Eu nunca tinha visto este desafio antes e não sabia como fazê-lo , então tive que procurar algo parecido , não achei com javascript , mas achei com a linguagem C , que estava [aqui](https://www.javatpoint.com/star-program-in-c) , porém o desafio exige que seja feito com Javascript e não C, então usei a lógica que foi aplicada na linguagem C e converti para Javascript.
Linguagens de programação usam a mesma lógica , porém a sintaxe muda e com isso a forma de estruturar o código.

Código feito com C:
```
    #include <stdio.h>  
    int main()  
    {  
        int n;  
        printf("Enter the number of rows");  
        scanf("%d",&n);  
        for(int i=1;i<=n;i++)  
        {  
            for(int j=1;j<=n;j++)  
            {  
                if(i==1 ||i==n||j==1||j==n-i+1||i==j||j==n)  
                {  
                printf("*");  
                }  
                else  
                {  
                      
                          printf(" ");  
                      }  
                     
                }        
            printf("\n");  
        }  
          
        return 0;  
    }  

```

## [Pasta print](https://github.com/devartes/desafio/tree/master/print)

> Basicamente o resultado do código é imprimido(print) no console. 

```
let n = 20; 
let string = "";

for(let i=1;i<=n;i++)  
{  
    for(let j=1;j<=n;j++)  
    {  
        if(i==1 ||i==n||j==1||j==n-i+1||i==j||j==n)  
        {  
          string += "#";
        }  
        else  
        {  
              
          string += " ";
              }  
             
        }  
              
        string += "\n"; 
}  

console.log(string);
```

  `let n = 20;` define o tamanho da ampulheta.

<img align="center" alt="png" src="https://github.com/devartes/desafio/blob/master/print.png?raw=true" width="400" style="max-width:100%">


## [Pasta window prompt](https://github.com/devartes/desafio/tree/master/window%20prompt)

## Como visualizar o resultado?

> Eu tive que usar html , para que o resultado fosse exibido no navegador , é necessário uma extensão como Live Server no Vs Code para visualizar o contéudo no navegador, quando a tela carregar vai aparecer uma caixa com uma mensagem "digite o tamanho para a ampulheta" e um espaço para que o tamanho seja digitado, como na imagem abaixo por exemplo:

<img align="center" alt="png" src="https://github.com/devartes/desafio/blob/master/window%20prompt%201.png?raw=true" width="400" style="max-width:100%">

> Você pode digitar um tamanho, exemplo : 20 ou 10 ou 30 ,etc , qualquer valor (número) e o resultado será exibido. </br>
> Para visualizar o resultado , será necessário inspecionar a página ou seja abrir o developer tools , para isso basta clicar com o botão direito do mouse e clicar inspecionar , como mostra a imagem abaixo:

<img align="center" alt="png" src="https://github.com/devartes/desafio/blob/master/window%20prompt%202.png?raw=true" width="400" style="max-width:100%">

> Uma segunda área será exibida , clique na aba "console" e o resultado estará lá.

<img align="center" alt="png" src="https://github.com/devartes/desafio/blob/master/window%20prompt%203.png?raw=true" width="400" style="max-width:100%">

> Diferente do código da [Pasta print](https://github.com/devartes/desafio/tree/master/print), o código da [Pasta window prompt](https://github.com/devartes/desafio/tree/master/window%20prompt) permite ao usuário definir o tamanho desejado para a ampulheta , esta parte do código é responsável por este processo :

```

let string = "";
let n = window.prompt('Digite um tamanho para a ampulheta ');

```
e
```
console.log(string + "\n" + "n= " + n);

```
que está aqui :

```
let string = "";
let n = window.prompt('Digite um tamanho para a ampulheta ');


for(let i=1;i<=n;i++)  
{  
    for(let j=1;j<=n;j++)  
    {  
        if(i==1 ||i==n||j==1||j==n-i+1||i==j||j==n)  
        {  
          string += "#";
        }  
        else  
        {  
              
          string += " ";
              }  
             
        }  
              
        string += "\n"; 
}  


console.log(string + "\n" + "n= " + n);

```
> dentro do [window prompt.js](https://github.com/devartes/desafio/blob/master/window%20prompt/window%20prompt.js)

> Eu não consegui realizar uma animação com os # e nem preencher o espaço inferior , fiz dois códigos , porém deixo para que o avaliador escolha qual dos dois será levado em consideração.
