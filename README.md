#  Joc de Șah în Java

Implementare a jocului clasic de șah, dezvoltată în Java ca proiect pentru cursul de **Programare Orientată pe Obiecte (POO)**. Proiectul pune accent pe modelarea pieselor și a tablei de joc folosind principiile fundamentale ale POO.

##  Descriere

Aplicația permite jucarea unei partide complete de șah între doi jucători, respectând regulile oficiale de mutare ale fiecărei piese. Arhitectura este construită în jurul unei ierarhii de clase care modelează în mod natural entitățile din joc: tabla, piesele și jucătorii.

##  Funcționalități

- Modelarea celor 6 tipuri de piese (pion, tură, cal, nebun, regină, rege), fiecare cu logica proprie de mutare
- Validarea mutărilor conform regulilor șahului
- Detectarea situațiilor de **șah** și **șah mat**
- Alternarea automată a turelor între cei doi jucători (alb / negru)
- Reprezentarea și actualizarea tablei de joc după fiecare mutare
- Capturarea pieselor adversarului

##  Concepte POO utilizate

Proiectul ilustrează principiile esențiale ale programării orientate pe obiecte:

- **Încapsulare** – fiecare clasă gestionează propria stare și expune doar metodele necesare
- **Moștenire** – piesele extind o clasă/abstractizare comună (`Piesa`), reutilizând logica generală
- **Polimorfism** – fiecare piesă își suprascrie metoda de validare a mutărilor (`muta` / `mutareValida`)
- **Abstractizare** – clasa de bază pentru piese definește un contract comun, fără a impune o implementare unică

##  Tehnologii

- **Java** (JDK 17 sau o versiune compatibilă)
- Programare orientată pe obiecte

##  Rulare

Clonează repository-ul și compilează sursele:

```bash
git clone https://github.com/utilizator/nume-proiect.git
cd nume-proiect
javac -d bin src/*.java
java -cp bin Main
```

> Înlocuiește `Main` cu numele clasei care conține metoda `main`, dacă diferă.

##  Structura proiectului

```
src/
├── Main.java          # Punctul de intrare în aplicație
├── Tabla.java         # Reprezentarea și gestionarea tablei de joc
├── Piesa.java         # Clasa de bază (abstractă) pentru piese
├── Pion.java          # Logica specifică pionului
├── Tura.java          # Logica specifică turei
├── Cal.java           # Logica specifică calului
├── Nebun.java         # Logica specifică nebunului
├── Regina.java        # Logica specifică reginei
└── Rege.java          # Logica specifică regelui
```

##  Posibile îmbunătățiri

- Interfață grafică (Swing / JavaFX)
- Mod de joc împotriva calculatorului
- Salvarea și încărcarea partidelor

##  Autor

Proiect realizat de Părău Leonard-Adrian
