# LogicaComputacional-S2-2024-3011542413035
Nome: Roger Willian
Email: roger13willian@gmail.com
GitHub: rogerwns
RA: 3011542413035


#código
n = 0
print("P | Q | R | S | P→Q | R→S | P∨R | (P→Q)∧(R→S)∧(P∨R) | Q∨S | ((P→Q)∧(R→S)∧(P∨R))→(Q∨S)")
 
for z in range(0, 2):
    for y in range(0, 2):
        for x in range(0, 2):
            for d in range(0, 2):
                if z == 0:
                    P = "V"
                else:
                    P = "F"
 
                if y == 0:
                    Q = "V"
                else:
                    Q = "F"
 
                if x == 0:
                    R = "V"
                else:
                    R = "F"
 
                if x == 0:
                    S = "V"
                else:
                    S = "F"
 
                if P == "F" or Q =="V":
                    PQ = "V"
                else:
                    PQ = "F"
 
                if R == "F" or S =="V":
                    RS = "V"
                else:
                    RS = "F"
 
                if P == "V" or R =="V":
                    PR = "V"
                else:
                    PR = "F"
 
                if PQ =="V" and RS == "V":
                    PQRS = "V"
                else:
                    PQRS = "F"
                             
                if PQRS =="V" and PR == "V":
                    PQRSPR = "V"
                else:
                    PQRSPR = "F"
 
                if Q == "V" or S == "V":
                    QS = "V"
                else:
                    QS = "F"
 
                if PQRSPR == "F" or QS == "V":
                    DC = "V"
                else:
                    DC = "F"
               
                print(f"{P} | {Q} | {R} | {S} |  {PQ}  |  {RS}  |  {PR}  |          {PQRSPR}         |  {QS}  |          {DC}          ")
               
                if DC == "V":
                    n += 1


# Trabalho finalizado
