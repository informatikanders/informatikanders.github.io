---
layout: post
title:  "Computersysteme Teil 1"
date:   2022-07-01 15:15:03 +0200
categories: jekyll update
---

yoyo in dieser Serie werde ich erläutern wie Computer (nicht Betriebssysteme!!!) richtig funktionieren. Wir fangen einfach an und enden komplex, jedoch wird das Komplexe einfach zu verstehen sein.
Zuallererst definieren wir, was wir überhaupt benutzen, um Computer abzubilden.
Wir benutzen in unserem Fall, da wir keine Elektrotechnik lernen, die Schaltalgebra.
Was ist die Schaltalgebra?

Die Schaltalgebra besteht im Grunde genommen aus einer Menge der Zahlen [0,1].
Diese haben die Regeln der Bool'schen Algebra übernommen, die wir später erwähnen.

![](/assets/img/Eigenschaften_boolsche_algebra.JPG)

Am Anfang betrachten wir jetzt Schaltnetze.

Was sind Schaltnetze?

Schaltnetz ist ein Schaltwerk, dessen Wert am Ausgang nur vom Wert am Eingang abhängt.

Wie können Schaltnetze entworfen werden?

![](/assets/img/Blockschaltbild.JPG)

Welche Eigenschaften charakterisieren die Schaltalgebra?

1. Es existiert eine Menge B = {0,1}
2. Es existieren die Verknüpfungen (Operatoren) UND, ODER, NICHT
3. Es gelten die Gesetze der Boolschen Algebra

![](/assets/img/Schaltzeichen.JPG)

Da wir nun wissen was die Eigenschaften der Schaltalgebra und was Schaltnetze sind, können wir easy peasy ganz einfach Schaltnetze erstellen.
Dabei gucken wir uns die Basisverknüpfungen an.

![](/assets/img/grundverknüpfung.JPG)

Somit haben wir jetzt die Möglichkeit aus diesen Grundverknüpfungen, die wichtigstens Verknüpfungen der Digitalelektronik zu bilden.

![](/assets/img/verknüpfungen_digitalelektronik.JPG)

Sofern so gut. Doch was machen wir jetzt weiter? Wie stellen wir das alles dar?

Dazu haben wir 5 Möglichkeiten: Wir stellen das als Funktionstabelle, Funktionsgleichung, KV-Diagramm, Schaltzeichen oder Binäres Entscheidungsdiagramm dar.

Fangen wir mit der Funktionstabelle an.

Was ist eine Funktionstabelle?

Eine Funktionstabelle ist eine Zusammenstellung aller möglichen Wertekombinationen der Eingangsvariablen und der zugehörigen Werte der Ausgangsvariablen
