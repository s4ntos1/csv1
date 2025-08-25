import csv 
lista = open("dados.csv")
arquivo = csv.DictReader(lista)
for carros in arquivo:
    if carros["Marca"] =="Ford":
       print(carros)
lista = open("dados.csv")
arquivo = csv.DictReader(lista)
for carros in arquivo:
    if carros ["Ano"] == "2020":
       print(carros)
lista = open("dados.csv")
arquivo = csv.DictReader(lista)
for carros in arquivo:
    if carros ["Valor"]  < "50.000":
       print(carros)
with open("dados.csv", "a" , newline="")as arquivo:
    escritor = csv.writer(arquivo)
    escritor.writerow (["Nissan", "Sky Line", "2012","30.000"])
