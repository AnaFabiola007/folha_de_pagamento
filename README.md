# folha_de_pagamento
#COM CALCULO DE IR

nome = input ("Digite o nome do funcionário: ")
print ("Nome do funcionário é", nome, "\n")

salariob = float(input("Qual o atual salário bruto do funcionário? "))
print (f"o seu salário bruto de {nome} é {salariob}")

if salariob <= 1302.00:
    perc =  7.5

elif salariob <= 2571.29:
    perc = 9
    INSS = 19.80

elif salario <= 3856.94:
    perc = 12
    INSS = 96.94

elif salario <= 3856.94:
    perc = 14
    INSS = 174.08

else:
    salario > 7507.49
    perc = 14
    INSS = 876.95
    
VT = float(input("deseja vale transporte? (1-sim ou 2-não) "))

if VT == 1:
    perc = perc + 6
elif VT != 1:
    perc = perc
    
if salariob >= 1903.99 <= 2826.65:
    perc =  perc + 7.5
    IR = 142.80

elif salariob <= 2571.29:
    perc = perc + 15
    IR = 354.80

elif salariob <= 3856.94:
    perc = perc + 22.5
    IR = 636.13

else:
    salariob > 3856.94
    perc = perc + 27.5
    IR = 869.36

    
liquido = (IR+INSS+salariob-(salariob*perc)/100)
print (f"O salário liquido de {nome} é {liquido}")
