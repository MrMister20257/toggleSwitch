# Toggle Switch Aufbau und Erklärung

## Was ist ein ToggleSwitch und warum funktioniert das?

Ein ToggleSwitch ist ein kleiner Hack in dem wir das Verhalten einer Checkbox in Verbindung mit einem Label nutzen um andere HTML-Elemente zu beeinflussen.

Wie wir bereits wissen kann man ein Label, durch die Verwendung von `for` und `id`, mit einem Inputfeld verknüpfen. Durch diese Verknüpfung ist es möglich das Inputfeld anzusprechen, durch das klicken auf das Label. Dies funktioniert mit allen types von Labels, daher auch mit `type="checkbox"`, auch wenn die Checkbox durch `display: none` versteckt ist.

Nun verwenden wir das klickbare Label `<label>Klick mich!</label>` um mit CSS-Selektoren Nachbar-Elemente zu beeinflussen.

**_Ein Vorteil dieses CSS-Hacks ist es, dass für dieses verhalten kein Javascript verwendet wird, wodurch es auch offline funktioniert._**

## Anleitung

Einen Toggle-Switch zu erstellen besteht aus 4 Schritten.

Schritt 1: Wir brauchen einen Container, hierfür eignet sich ein Label, da nur dieses eine Checkbox ansprechen kann.

Schritt 2: Wir benötigen eine Checkbox, die wir mit display: none unsichtbar machen.

Schritt 3: Wir benötigen Content, den wir komplett fertig stylen! Der content conatiner MUSS auf der selben Ebene sein, wie die checkbox!

Schritt 4: Wir sagen (im CSS) was geschehen soll, wenn Checkbox = checked ist, Beliebt sind änderungen der display Eigenschaften oder der width/height

## Beispiel

```
  <label>
    <input type="checkbox" id="name">
    <p>Anklickbares Element/Überschrift/Icon/:befor/:after</p>
    <ul>
      <li>Content...</li>
    </ul>
  </label>
```

## Aufgabe

**BILD 1**

1. Baue einen `boxContainer1` der zwei `article` mit Beispieltext beinhaltet
2. In diesem `boxContainer1` sollen 2 unabhänge `tootleSwitch` Boxen zu sein. Bei einem Klick auf den Titel (das Lebel) soll sich der Content auf und zu klappen
3. Versuche, dass die erste Box bei einem Klick ein und ausgeblendet wird
4. Versuche dass die zweite Box bei einem Klick langsam auf- und zugeht.

### Bonus (Achtung Knobelaufgabe!)

**BILD 2**

1. Erstelle einen `boxContainer2` der ebenfalls zwei `article` mit Beispieltext enthält
2. Versuche nun das Verhalten der `article` so anzupassen, dass nur einer der beiden `article` angezeigt wird.

<details>
<summary>Tipp?</summary>
<br>
Denke daran, dass ein Label mit allen Types eines Inputs verlinkt werden kann.
</details>
