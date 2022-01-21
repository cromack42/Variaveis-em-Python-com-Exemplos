# Variaveis-Globais-em-Python-com-exemplos

Um resumo traduzido para o português do site SimpliLearn. 

###
Apresentação:
_____________________________________________________________________________________________
  Olá mundão, 
  
Me chamo Marcelo e sou desenvolvedor Python.
    Durante meus dias de aprendizado venho constantemente voltando o aprendizado em alguns conceitos acerca da linguagem e
    pensando em aprender de uma forma dinâmica, me veio a intenção de traduzir um artigo em um site extrangeiro no qual muito me agradou a forma de aprendizado.
    O endereço do site virá abaixo e peço mque qualquer um se sinta livre para usar, modificar e alterar, em qualquer instlancia minha tradução.
   Deixo claro que entarei ao máximo mnater a coêrencia e a uniformidade no meu trabalho, tentando manter a extrutura da linguagem inalterada.
  
______________________________________________________________________________________________
  
  
Qual é a variável global em python?
  
  No mundo da programação, uma variável global em Python significa ter um escopo ao longo do programa, 
  ou seja, um valor variável global é acessível em todo o programa, a menos que seja sombreado.  
  Em outras palavras, variáveis que são declaradas fora de uma função, são conhecidas como variáveis globais.


    Syntax:
    X = “SimplesValorGlobal”
    Def fn1():
    
______________________________________________________________________________________________

Como criar uma variação global em Python?

  Para criar uma variação em Python, você pprecisa declarar a variável fora da função ou em um âmbito global
  
Exemplo: 

    x = "Primeira Variante Global" #declarando a variação Global
    
    def myfunc():
      print("Valor da variante global em Python é: " + x)
    myfunc()  
    
Saída:

    PS C:\Users\VRAME2> python -u "c:\Users\VRAME2\Desktop\Variante Global.py"
    Valor da Variante Global em Python é: Primeira Variante Global
    PS C:\Users\VRAME2
_____________________________________________________________________________________________

Como acessar a variante global dentro e fora da função?

Exemplo: 

    x = "Primeira Variante Global" #Declarando Variante Global
    
    def myfunc():
      print("Acessando a função dentro: " + x)
      
    myfunc()
    print("Acessando a função fora: " + x)
    
 Saída:
 
    PS C:\UsersVRAME2> python -u "c:\Users\VRAME2\Desktop\Variável Global.py"
    Acessando uma função de dentro: Primeira Variável Global
    Acessando uma função de fora: Primeira Variável Global
    ps C:\Users\VRAME2>
    
 No exemplo descrito acima, você viu uma variável global declarada e 
 acessada dentro e fora da função.
 
 Então, se você acessar ambos os valores dentro e fora da função, isso é bom, mas o que acontece 
 se você tentar modificar o valor da variável de escopo global dentro de uma função?
 
 Veja o exemplo mencionado para entender melhor.
 
 Exemplo:
 
    x = "5" #Declarando uma Variável Global
    
    def myfunc():
        x = x * 2 #Modificando o valor da variável dentro da função.
        print("Acessando a função de dentro: "+ x)
    myfunc()
    print("Acessando a função de fora: " + x)
    
 saída:
 
    PS C:\Users\VRAME2> python -u "c:\Users\VRAME2\Desktop\Variavel Global.py"
    Traceback (most recent call last):
    File "c:\Users\VRAME2\Desktop\Variavel Global.py", line 7, in <module>
      myfunc()
    File "c:\Users\VRAME2\Desktop\Variaveis Globais.py", line 4, in myfunc
      x = x * 2 modificando o valor da função dentro da variavel global.
    UnboundLocalError: variável local 'x' referenciada antes da atribuição
    PS C:\Users\VRAME2>
    
    
