**inicio da aula, n dei um titulo**  
F(Base,Precisão,MenorExpoente,MaiorExpoente)  
  => sinal é implicito  
  => normalizado é implicito  
ex:  
  12,3 => F(10,3,x,y) => fl(x) 
  1,23 => F(10,3,x,y)  
  0,123 => F(10,3,x,y)
    => nese caso o professor usou {-2, 2}, mas acredito q um valor dado  

+-(+- expoente) mantiça 
  => mantiça = valores do numero  
    => expoente entram sem o sinal  
ex:  
  12,3 => +(+2)123  
  1,23 => +(+1)123  
  ,123 => +(+0)123  

**IEEE**  
  Base: 2  
  F(2,x,y,z)  

ex:  
  F(2,23,-126,+127),como a base é 2, 23 de precisão significa q temos q usar 32 bits  
  F(2,33,-1022,+1023),como a base é 2, 33 de precisão significa q temos q usar 64 bits  

**Numeros ñ representaveis**  

Truncamento:Apaga todo número que exceda a representação/escala.  

Arredondamento:vc ja sabe. >=5 = +1 (Se não for indicado, é arredondamento)  

**Operações**  
⊕ ⊖ ⊗ ⊘ "bolinha" escrever e pegar os simbolos  
    => eles indicam a inclusão do fl()  

ex:  
    x ⊕ y = fl(fl(x) + fl(y))  

    x ⊖ y ⊕ z (colocar os simbolos corretos)  
        fl((fl(x) - fl(y)) ⊕ z)  
        fl(fl(fl(x) - fl(y)) + fl(z))  

**Norma**  
Norma 1  

Norma Euclidiana  

Norma de máximo ou infinito  

**Zero de Funções/Metodo de Newton**   
Método da Bisseção  

Método da Falsa Posição  

Método de Newton  
    tan(x)=(f(x0) - 0)/(x0-x1) #achar os simbolos pra x0 e etc  
    x0 é dado SEMPRE  
    x1=x0- (f(x0)/f'(x0))           |   f'(x0)!= 0  
    x2=x1- (f(x1)/f'(x1))           |   f'(x1)!= 0  
    xn= xn-1 - (f(xn-1)/f'(xn-1))   |   f'(xn)!= 0  

obs:  
    o Método de newton pode ser escrito (usando algebrismo) como;  
        xn = ((xn-1*f(xn-1))-f(xn-1))/f'(xn-1)  

**Metodo da Secante**

    x0,x1 são dados  
    x2= (x1*f(x0)-x0*(f(x1)))/(f(x0)-f(x1))  
    x3= (x2*f(x1)-x1*(f(x2)))/(f(x1)-f(x2))  
    xn= (xn-1*f(xn-2)-xn-2*(f(xn-1)))/(f(n-2)-f(xn-1))  
