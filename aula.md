__inicio da aula, n dei um titulo__
F(Base,Precisão,MenorExpoente,MaiorExpoente)
  => sinal é inplicito
  => normalizdo é inpicito
ex:
  12,3 => F(10,3,x,y) => fl(x)
  1,23 => F(10,3,x,y)
  ,123 => F(10,3,x,y)
    => nese caso o professor usou {-2, 2}, mas acredito q um valor dado

+-(+- expoente) mantiça
  => mantiça = valores do numero
    => expoente entram sem o sinal
ex:
  12,3 => +(+2)123
  1,23 => +(+1)123
  ,123 => +(+0)123

__IEEE__
  Base: 2
  F(2,x,y,z)

ex:
  F(2,23,-126,+127),como a base é 2, 23 de precisão significa q temos q usar 32 bits
  F(2,33,-1022,+1023),como a base é 2, 33 de precisão significa q temos q usar 64 bits

__Numeros ñ representaveis__

Truncamento:Apaga todo número queexceda a representação/escala.

Arredondamento:vc ja sabe. >=5 = +1 (Se não for indicado, é arredondamento)

__Operações__
+-*/ "bolinha" escrever e pegar os simbolos
    => eles indicam a inclusão do fl()

ex:
    x-y+z (colocar os simolos corretos)
        fl(fl(x) - fl(y)) + z
        fl(fl(fl(x) - fl(y)) + fl(z))
