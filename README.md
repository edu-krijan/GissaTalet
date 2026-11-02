# GissaTalet
Övning
import random

def gissa_talet():
    hemligt_tal = random.randint(1, 100)
    forsok = 0
    
    print("Välkommen till 'Gissa talet'!")
    print("Jag tänker på ett tal mellan 1 och 100. Kan du gissa vilket?")
    
    while True:
        gissning = int(input("Skriv din gissning: "))
        forsok += 1
        
        if gissning < hemligt_tal:
            print("För lågt! Prova ett högre tal.\n")
        elif gissning > hemligt_tal:
            print("För högt! Prova ett lägre tal.\n")
        else:
            print(f"Rätt! Du klarade det på {forsok} försök!")
            break

gissa_talet()