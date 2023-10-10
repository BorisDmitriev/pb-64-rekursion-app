# Schul-App
* erstelle eine App zum Hinzufügen, Entfernen, Lesen und Bearbeiten von Schülern und Klassen in einer Schule

   * das Schulmodell:
  ```js
     School=[ classObject1,classObject2,....]
  ```

   * das Klassenmodell:
   ```js
    {
        Name: "FbW3",
        students: [studentObject1, studentObject2,...],
    }
    ```

    * das Schüler-Modell:
  
    ```js
    {
            name: "Pilar",
            email: "pilar@yahoo.com",
            city: "Berlin",
    }
    ```

Schul-Datenmodell:
```js
 [
  {
    name: "FbW1",
    students: [
      {
        name: "Alex",
        email: "alex@yahoo.com",
        city: "Berlin",
      },
      {
        name: "Max",
        email: "max@yahoo.com",
        city: "Hamburg",
      },
    ],
  },

  {
    name: "FbW2",
    students: [
      {
        name: "Jon",
        email: "jon@yahoo.com",
        city: "Berlin",
      },
      {
        name: "Pilar",
        email: "pilar@yahoo.com",
        city: "Berlin",
      },
    ],
  },
  {
    name: "FbW3",
    students: [],
  },
]
```




### Aufgaben
## Aufgabe1: Eine Klasse erstellen:
- Erstelle eine Funktion namens `createClass`, um eine neue Klasse hinzuzufügen.
- Die Funktion `createClass` sollte ein Argument (Objekt) erhalten, das den Namen der Klasse `name` und ein leeres Array für `students` enthält.

## Aufgabe2: Hinzufügen eines Schülers:
- Erstelle eine Funktion namens `createStudent`, um einen neuen Schüler hinzuzufügen.
- Die Funktion `createStudent` sollte ein Argument (Objekt) erhalten, das *Schülerdaten* enthält.
- Die Schülerdaten sollten wie der folgende Beispielcode aussehen:
```js
  {
        classID: 21,
        name: "Pilar",
        email: "pilar@yahoo.com",
        city: "Berlin",
  }
 ```
## Aufgabe3: Entfernen einer Klasse:
- Erstelle eine Funktion zum Entfernen der Klasse und nenne sie `removeClass`.
- Die Funktion `removeClass` sollte ein Argument namens `classID` für die ID der Klasse erhalten.

## Aufgabe 4: Entfernen eines Schülers:
- Erstelle eine Funktion namens `removeStudent`, um einen Schüler aus einer Klasse zu entfernen.
- Die Funktion `removeStudent` sollte ein Argument (Objekt) erhalten, das `classID` für die ID einer Klasse und `studentID` für die ID eines Schülers enthält.

## Aufgabe5: Einen Schüler bearbeiten:
- Erstelle eine Funktion zum Bearbeiten eines bestehenden Schülers und nenne sie `editStudent`.
- Die Funktion `editStudent` sollte ein Argument (Objekt) annehmen, das `classID` für die ID der Klasse, `studentID` für die ID des Schülers, `email` für die E-Mail des Schülers, `city` für die Stadt des Schülers und `name` für den Namen des Schülers enthält. __Vergewissere dich, dass du die genauen Namen der Objektwerte verwendest__.

## Aufgabe6: Rendering der Schuldaten:
- Erstelle eine Funktion zum Rendern der Schuldaten und nenne sie `RenderSchoolTemplate`.
- Die Funktion `RenderSchoolTemplate` sollte die Schuldaten als String zurückgeben, der so formatiert ist wie unten:
```js
 Schulklassen:
------------------
 FbW1 - (Klassen-ID: 1):
  1- Alex, alex@yahoo.com, Berlin - (Schüler ID: 1).
  2- Max, max@yahoo.com, Hamburg - (Schüler-ID: 2).
********************************************
 FbW2 - (Klassen-ID: 2):
  1- Jon, jon@yahoo.com, Berlin - (Schüler-ID: 1).
  2- Pilar, pilar@yahoo.com, Berlin - (Schüler-ID: 2).
********************************************
 FbW3 - (Klassen-ID: 3):
   Die Klasse ist leer
********************************************
  Klassen insgesamt 3, Schüler insgesamt 4
```
