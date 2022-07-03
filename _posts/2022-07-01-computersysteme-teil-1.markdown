---
layout: post
title:  "Computersysteme Teil 1"
date:   2022-07-01 15:15:03 +0200
categories: jekyll update
---

yoyo in dieser Serie werde ich erläutern wie Computer (nicht Betriebssysteme!!!) richtig funktionieren. Wir fangen einfach an und enden komplex, jedoch wird das Komplexe einfach zu verstehen sein.
Zuallererst definieren wir, was wir überhaupt benutzen, um Computer abzubilden.
Wir benutzen die Schaltalgebra.
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

Eine Funktionstabelle ist eine Zusammenstellung aller möglichen Wertekombinationen der Eingangsvariablen und der zugehörigen Werte der Ausgangsvariablen.

Sind für alle möglichen Wertekombinationen der Eingangsvariablen, Werte für die Ausgangsvariablen festgelegt, dann spricht man von einer vollständigen Funktionstabelle. In einer unvollständigen Funktionstabelle ist nicht für jede mögliche Eingangskombination ein fester Wert der Ausgangsvariablen festgelegt.

![](/assets/img/funktionstabelle.JPG)

Wie können wir Schaltnetze als Funktionsgleichung darstellen?

Im Allgemeinen können wir diese als y = f(a,b,c) darstellen, dabei werden die Argumentvariablen mit Operatoren UND,ODER,NICHT verknüpft.

Siehe folgendes Bild als Beispiel:

![](/assets/img/Funktionsgleichung.JPG)

Des Weiteren sind folgende Regeln hilfreich bei Umformungen von Schaltfunktionen:

![](/assets/img/umformung_schaltfunktionen.JPG)

Wir gucken uns jetzt an, wie Schaltnetze in der Normalform dargestellt werden können.

Es gibt zwei Möglichkeiten die Schaltnetze in der Noramlform darzustellen

1.Disjunktive Normalform (DNF)
2.Konjuktive Normalform (KNF)

Worin unterscheiden sich die beiden?

Die Disjunktive Normalform einer Schalfunktion ist eine Disjunktion (ODER-Verknüpfung) von Mintermen.
Jeder Minterm ist dabei eine Konkjuktion, die jede Eingangsvariable negiert oder nicht negiert enthält.
Besteht eine Schaltfunktion aus Disjunktionen von Konjuktionstermen, die nicht alle Eingangsvariablen enthalten, so spricht man von einer disjunktiven Form (DF).

Die Konjuktive Normalform einer Schaltfunktion ist eine Konjuktion (UND-Verknüpfung) von Maxtermen. Jeder Maxterm ist dabei eine Disjunktion,
die jede Eingangsvariable negiert oder nicht negiert enthält. Besteht eine Schaltfunktion aus Konjunktionen von Disjunktionstermen, die nicht alle Eingangsvariablen enthalten, so spricht man von einer konjunktiven Form (KF).

So sieht eine Tabelle aus, die alle Kombinationen aus zwei Schaltvariablen zeigt und die möglichen Minterme mit ihren zugehörigen Werten:

![](/assets/img/dnf_tabelle.JPG)

So sieht eine Tabelle aus, die alle Kombinationen aus zwei Schaltvariablen zeigt und die möglichen Maxterme mit ihren zugehörigen Werten:

![](/assets/img/knf_tabelle.JPG)

Dabei sieht die Schaltfunktion der DNF wie folgt aus:

![](/assets/img/schaltfunktion_dnf.JPG)

Und die Schaltfunktion der KNF so:

![](/assets/img/schaltfunktion_knf.jpg)

Als Nächstes betrachten wir die Karnaugh-Veitch-Diagramme, auch KV-Diagramme genannt.

Diese Diagramme sind ein grafisches Tool zur Darstellung von Wertetabellen oder Schaltfunktionen.

![](/assets/img/funktiontabelle_und_kvdiagramm.JPG)

Beispielsweise soll folgende Schaltfunktion in der DNF als KV-Diagramm gezeichnet werden:

![](/assets/img/dnf_beispiel_kv.JPG)

So sieht dann das Resultat aus (die Minterme sind wie o.g. als 1 hinterlegt, der Rest wird mit 0 gefüllt):

![](/assets/img/kv_diagramm_dnf.JPG)

Das Gleiche kann man mit einer Schaltfunktion in KNF machen:

![](/assets/img/knf_beispiel_kv.JPG)

Und anbei das Resultat (die Maxterme sind wie o.g. als 0 hinterlegt, der Rest wit mit 1 gefüllt):

![](/assets/img/kv_diagramm_knf.JPG)

Wozu brauchen wir die KV-Diagramme?

Diese werden später hilfreich sein beim Vereinfachen von Schaltfunktionen und bei der Übertragung einer Funktionstabelle in eine Funktionsgleichung.

Jetzt kommen wir zur Darstellung durch Schaltzeichen.

Warum brauchen wir Schaltzeichen?

Einerseits um später  die technischen Systeme graphisch darzustellen und andererseits um mithilfe von der Schaltzeichen, die Systeme analysieren zu können.

Gucken wir uns ein Beispiel an, wie wir eine Schaltfunktion, mithilfe der Schaltzeichen darstellen können:

Die Schaltfunktion:

![](/assets/img/funktion_schaltzeichen.JPG)

dargestellt mithilfe von Schaltzeichen:

![](/assets/img/schaltzeichen_system.JPG)

Kommen wir zur Minimierung der Schaltfunktionen.

Wozu brauchen wir die?

Die Minimierung benötigen wir, um redundante Terme in Schaltfunktionen zu entfernen, da diese aus der Sicht der Chiphersteller, extrem kostenaufwendig sind.

Diese Terme können entfernt werden, da sich die Arbeitsweise der Chips bzw. später des Computers sich nicht verändert.

Hier kommen die vorhin erwähnten Regeln der Minimierung ins Spiel.

So ist beispielsweise folgende Funktionsgleichung:

![](/assets/img/minimierung_gleichung.JPG)

äquivalent zu folgender Gleichung:

![](/assets/img/äquivalent_gleichung.JPG)

Es gibt verschiedene Verfahren, wie Gleichungen minimiert werden können.

Grundlage aller Verfahren gelten folgende zwei Gesetze der Schaltalgebra:

![](/assets/img/zwei_gesetze.JPG)

Die wichtigsten Verfahren lauten:

- Anwendung der Gesetze der Schaltalgebra
- KV-Diagramme
- Methode von Quine-McCluskey

Verfahren mit den Gesetzen der Schaltalgebra

Hier kann durch Ausklammern von Variablen, Kürzen, Zusammenfassen, Anwendung der De Morganschen Gesetze eine Schaltfunktion vereinfacht werden.

Beispiel:

![](/assets/img/vereinfachung_gesetze.JPG)

Verfahren mit KV-Diagramm:

Dieses Verfahren ist grafisch. Wenn das KV-Diagramm eine Schaltfunktion in DNF darstellt, dann werden die benachbarten Felder, die mit 1 belegt sind, zusammengefasst. Wie findet die Zusammenfassung statt? Diese findet so statt, dass möglichst viele Einsen eingeschlossen werden. Dabei dürfen nur rechteckige
Blöcke gebildet werden (das bedeutet, es dürfen nur eins, zwei, vier, acht usw. Felder entstehen). Felder der ersten
und letzten Zeile aber gleicher Spalte sind benachbart und können in einem Block zusammengefasst werden; ebenso Felder der ersten und letzten Spalte
aber gleicher Zeile. Die vereinfachte Schaltfunktion wird dann aus den Termen der zusammengefassten Blöcke und der übriggebliebenen Einzelfelder gebildet.
Die Terme der zusammengefassten Blöcke enthalten nur die Variablen, die sich innerhalb eines Blockes nicht ändern.

Anbei ein KV-Diagramm, dass die Schaltfunktion in DNF darstellt und die mit 1 belegten Felder zusammenfasst:

![](/assets/img/grafisch_kv_diagramm.JPG)

Die vereinfachte Schaltfunktion lautet:

![](/assets/img/vereinfachte_schaltfunktion_dnf.JPG)

Jetzt ein KV-Diagramm, dass die Schaltfunktion in KNF darstellt und die mit 0 belegten Felder zusammenfasst:

![](/assets/img/grafisch_knf_diagramm_kv.JPG)

und anbei die vereinfachte Schaltfunktion:

![](/assets/img/vereinfachte_schaltfunktion_knf.JPG)
