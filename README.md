# Pedra-Papel-ou-Tesoura-
Um jogo de Pedra, Papel ou Tesoura na linguagem Python

     
from random import randint
N = 3
V = []
D = []
E = []
P = int(input("Quantas partidas gostaria de jogar?\n"))
print ()

#situações
for x in range (1, P + 1):
 U = input("Pedra, Papel ou Tesoura?\n")
 U = U.title()
 U = U.strip()
 print ()

 I = randint(1,3)
 if I == 1:
  I = "Pedra"
 if I == 2:
  I = "Papel"
 if I == 3:
  I = "Tesoura"

 if (U == "Pedra" and I == "Tesoura" or U == "Papel" and I == "Pedra" or U == "Tesoura" and I == "Papel"):
   print ("{} vence {}. Você ganhou.".format(U,I))
   V.append(1)
   print ()
 if (U == "Pedra" and I == "Pedra" or U == "Papel" and I == "Papel" or U == "Tesoura" and I == "Tesoura"):
   print ("{} empata com {}. Vocês empataram.".format(U,I))
   E.append(1)
   print ()
 if (U == "Pedra" and I == "Papel" or U == "Papel" and I == "Tesoura" or U == "Tesoura" and I == "Pedra"):
   print ("{} perde pra {}. Você perdeu.".format(U,I))
   D.append(1)
   print()
print ("Houve {} vitória(s), {} empate(s), e {} derrota(s).".format(len(V), len(E), len(D)))
