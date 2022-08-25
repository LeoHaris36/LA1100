# Projekt-Dokumentation


Leo Haris Sljivar

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|       | 0.0.1   | ✍️ Jedes Mal, wenn Sie an dem Projekt arbeiten, fügen Sie hier eine neue Zeile ein und beschreiben in *einem* Satz, was Sie erreicht haben. |
|       | ...     |                                                              |
|       | 1.0.0   |                                                              |

## 1 Informieren

### 1.1 Ihr Projekt

Ich mache einen Number guesser bei dem man eine Zahl von 1-100 erraten muss

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1.0   |    Muss      |  Funktional    |  Als Spieler möchte ich eine Zufällige Zahl zwischen 1-100 damit ich eine Zahl zum raten habe und das Spiel anfangen kann.  |
| 2.0  |     Muss         |    Funktional     |    Als Spieler möchte ich eine Zahl eingeben damit ich raten und gewinnen kann.               |
| 3.1  |     Muss         |    Qualität     |      Als Spieler möchte ich wissen ob meine Zahl niedriger ist damit ich bessere Chancen habe die Zahl zu erraten       |
| 3.2  |         Muss     |  Qualität       |          Als Spieler möchte ich wissen ob meine Zahl höher ist damit ich bessere Chancen habe die Zahl zu erraten       |
| 3.3 |    Muss          |     Funktional    |    Als Spieler möchte ich wissen wann ich die richtige Zahl geraten habe.               |
| 4.0  |     Muss         |   Qualität      |   Als Spieler möchte ich wissen wie viele male ich geraten habe damit ich die Resultate vergleichen kann                |
| 5.0  | Muss | Funktional | Als Spieler möchte ich dass ich eine Fehlermeldung bekommen wenn ich etwas falsches eingegeben habe damit ich richtig spielen kann  |
| 6.0 | Kann | Qualität | Als Spieler möchte ich ein Punktesystem einführen, in welchem man seine Punkte wetten kann. Je mehr Veruche man braucht um die Zahl zu eraten desto weniger Punkte bekommt. Wenn man zu viele Versuche braucht gibt es minus Punkte, damit man mehr spass hat und mit anderen Punkte vergleichen kann.  |

### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |   Ich habe das Programm für die zufällige Zahl erstellt und gestartet           |    Start des Programmes     |      1*-100*          |
| 2.1  |    Das Programm ist gestartet und generiert die Zahl         |    Start des Programmes    |  Bitte geben Sie eine Zahl an                 |
| 3.1.1 | Das Programm ist gestartet, die Zahl ist generiert und sie werden nach einer Zahl gefragt | -5 | Zu tief! |
| 3.2.1 | Das Programm ist gestartet, die Zahl ist generiert und sie werden nach einer Zahl gefragt | 200 | Zu hoch!! |
| 3.3.1 | Das Programm ist gestartet, die Zahl ist generiert und sie werden nach einer Zahl gefragt | Richtige Zahl | Korrekt!! |
| 4.1 | Sie haben die richtige Zahl eraten | Richtige Zahl nach 4x versuchen | Die vorherigen 4x Zahlen |
| 5.1 | Das Programm fragt sie nach einer Zahl | Hallo | Keine Zahl erkannt = Selbszerstörung aktiviert |
| 6.1 | Das Programm startet, Sie haben Punkte und das Programm fragt sie ob Sie etwas wetten wollen | 10 | 10 Punkte im Pot, viel glück. |
| 6.2 | Sie spielen und brauchen nur einen Versuch  | Richtige Zahl* | Korrekt! Jackpot! +x Punkte |
| 6.3 | Sie spielen und brauchen 3 Versuche und machen somit Gewinn | Richtige Zahl* | Korrekt! Glückwunsch! +x Punkte |
| 6.4 | Sie spielen und brauchen 5 Versuche und machen somit Verlust | Richtige Zahl* | Korrekt! Sie verlieren jedoch x Punkte, the house always wins. |


### 1.4 Diagramme

![image](https://user-images.githubusercontent.com/111046405/186596607-ebfe1275-d260-4f77-b79f-7e63f471ed90.png)


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |  01.09     |     Sljivar      |       lernen wie man eine zufällige Zahl generiert, implemetieren, die Zahl lesen und festhalten      |      45min         |
| 2.A, 3.1A, 3.2A, 3.3A |  08.09     |  Sljivar  |    Die Eingabe des Spielers lesen und festhalten, und ein hinweissystem implemetieren damit ich weiss ob ich zu tief, zu hoch oder richtig gerraten habe.  |  45min |
| 3.1B, 3.2B, 3.3B | 08.09 | SLjivar | Einen Hinweis darauf geben ob man zu tief, zu hoch oder richtig geraten habe  | 45min |
| 3.1B, 3.2B, 3.3B | 08.09 | SLjivar | Einen Hinweis darauf geben ob man zu tief, zu hoch oder richtig geraten habe  | 45min |
| 4.A | 08.09 | Sljvar | Alle Resulte speichern und Anzeigen lassen | 45min |
| 4.B | 08.09 | Sljvar | Alle Resulte speichern und Anzeigen lassen | 45min |
| 5.A | 15.09 | Sljivar | Eine Lösung für eine Fehleingaben implementieren | 45min |
| 5.B | 15.09 | Sljivar | Eine Lösung für eine Fehleingaben implementieren | 45min |
| 6.A | 29.09 | SLjivar | Ein Punktesystem implementieren mit Wetten | 45min |
| 6.B | 29.09 | SLjivar | Ein Punktesystem implementieren mit Wetten | 45min |
| 6.C | 29.09 | SLjivar | Ein Punktesystem implementieren mit Wetten | 45min |
| 6.D | 29.09 | SLjivar | Ein Punktesystem implementieren mit Wetten | 45min |


## 3 Entscheiden

Ich Programmiere einen Number guesser der einem Hinweise darauf gibt ob die Zahl die man geraten hat zu tief oder zu hoch ist und wenn man die Zahl erraten hat man sieht was alles eingegeben wurde. Zusätzliches gibt es noch ein Punkte gambling System damit man um etwas spielt, die Punkte werden immer Angezeigt.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |       |           |               |                   |
| ...  |       |           |               |                   |

✍️ Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten.

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |              |         |                   |                      |
| ...  |              |         |                   |                      |

✍️ Verwenden Sie römische Ziffern für Ihre Bug Reports, also I, II, III, IV etc.

## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
