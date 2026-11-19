# grundlagen_informatik_1-uebung4
tasks for learning the language "Python"

Aufgabe1

Entwerfen Sie eine Funktion, welche die Quadratzahlen von 1^2 bis 20^2 ausgibt

Entwerfen Sie eine zweite Variante, bei der ein Startwert und ein Endwert für die Ausgabe bestimmt werden kann

Aufgabe 2

Schreiben S

#_____________________Aufgabe1_______________________
def Quadratzahl ():
    i=1
    while i<=20:
        print (f"Quadrat von {i}={i**2}")
        i=i+1
def Quadratzahl2 (start, ende):
    i=start
    while i<=ende:
        print (f"Quadrat von {i}={i**2}")
        i=i+1
#_____________________Aufgabe2_______________________
def Geradezahlen (n):
    i=1
    zahl=0
    while i<=2*n:
        if i%2==0:
            zahl=zahl+i
            i=i+1
        else:
            i=i+1
    print (f"{zahl}")
# Aufgabe 2 aus ohne Zähler
def summe_gerader_zahlen (anz):
    summe = 0
    while anz>0:
        if anz%2==0:
            summe=summe+anz
            anz=anz-1
        else:
            anz=anz-1    
    print(f"{summe}")
#_____________________Aufgabe3_______________________
def Rechteck (breite, hoehe):
    i=1
    while i<=hoehe:
        print('*'*breite)
        i=i+1
def Quadrat(breite):
    Rechteck(breite,breite)
#_____________________Aufgabe4_______________________
#_____________________Aufgabe5_______________________
def dreieck (hoehe):
    i=1
    while i<=hoehe:
        print('*'*i)
        i=i+1
def dreieck_mittig (hoehe):
    i=1
    while i<=hoehe:
        print(' '*(hoehe-i)+'*'*(i*2-1)+' '*(hoehe-i))
        i=i+1
def dreieck_hohl (hoehe):
    i=1
    while i<hoehe:
        if i==1:
            print(' '*(hoehe-i)+'*'+' '*(hoehe-i))
            i=i+1
        else:
            print(' '*(hoehe-i)+'*'+' '*(i*2-3)+'*'+' '*(hoehe-i))
            i=i+1
    print('*'*(hoehe*2-1))
#_____________________Aufgabe6_______________________
def quersumme (zahl):
    ergebnis=0
    while zahl: # bool kann auf zahlen gemappt werden, 0 wird automatisch "false"
        ergebnis=ergebnis+zahl%10
        zahl=zahl//10
    return ergebnis
#_____________________Aufgabe7_______________________
def zahl_gespiegelt (zahl):
    i=0
    originalzahl=zahl
    ergebnis=0
    while zahl:
        i=i+1
        zahl=zahl//10
    while originalzahl:
        i=i-1
        ergebnis=ergebnis+(originalzahl%10)*10**i
        originalzahl=originalzahl//10      
    return ergebnis
 #_____________________Aufgabe8_______________________   
def multiplikation_ohne_mal (faktor1, faktor2):
    ergebnis=0
    while faktor2:
        ergebnis=ergebnis+faktor1
        faktor2=faktor2-1
    return ergebnis
     
     
    
    
