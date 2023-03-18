from random import randint

V = []
D = []
E = []
P = int(input("Quantas partidas gostaria de jogar?\n"))
print ()

for x in range (1, P + 1):
 U = input("Pedra, Papel ou Tesoura?\n")
 U = U.title()
 U = U.strip()
 if U == "Pedra":
  U = "✊Pedra"
 if U == 'Papel':
  U = "✋Papel"
 if U == 'Tesoura':
  U = "✌️Tesoura"

 print ()

 I = randint(1,3)
 if I == 1:
  I = "✊Pedra"
 if I == 2:
  I = "✋Papel"
 if I == 3:
  I = "✌️Tesoura"

 if (U == "✊Pedra" and I == "✌️Tesoura" or U == "✋Papel" and I == "✊Pedra" or U == "✌️Tesoura" and I == "✋Papel"):
   print(U[0:1] + " × " + I[0:1])
   print ("✦ {} vence {}. Você ganhou. ✦".format(U[1::],I[1::]))
   V.append(1)
   print ()
 if (U == "✊Pedra" and I == "✊Pedra" or U == "✋Papel" and I == "✋Papel" or U == "✌️Tesoura" and I == "✌️Tesoura"):
   print(U[0:1] + " × " + I[0:1])
   print ("✦ {} empata com {}. Vocês empataram. ✦".format(U[1::],I[1::]))
   E.append(1)
   print ()
 if (U == "✊Pedra" and I == "✋Papel" or U == "✋Papel" and I == "✌️Tesoura" or U == "✌️Tesoura" and I == "✊Pedra"):
   print(U[0:1] + " × " + I[0:1])
   print ("✦ {} perde pra {}. Você perdeu. ✦".format(U[1::],I[1::]))
   D.append(1)
   print()
   
print ("Houve {} vitória(s), {} empate(s), e {} derrota(s).".format(len(V), len(E), len(D)))
   
