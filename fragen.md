1.Positionieren Sie zuerst alle Elemente lediglich mit position: absolute. Wodran
richten sich hierbei die Elemente aus? Inwiefern ändert sich das Verhalten, wenn das
Elternelement (<div>) auch ein position:absolute besitzt? Wie groß sind die
Boxen bei absoluter Positionierung? Was passiert mit den nachfolgenden (Geschwister-)
Elementen? Was für Probleme treten bei welchen Elementen auf, wenn Sie versuchen das
Wireframe lediglich mit absoluter Positionierung darzustellen?

Wenn es bei postion keine left,rigt,top,bottom gibt sind alle elemente auf top links orientret und auf einander.

Die Elemente orientrieren sich am Rand des nächsthöheren Elternelements. Wenn wir scrollen die Elementen bleiben wo sie sind (footer).
Wenn div auch absolute ist geht aside aus der Seite (ganz nach links),wenn es top,links... bei elementen gibt. 
Footer hat width 100%, andere nur so gross, dass das Text in sie passt.
Sibling elements bleiben unter ein ander, wie ohne absolute, jeder kann ein eingenes style haben (absolute.hmtl).
Problemen: mit footer, am bodem, wenn wir scrollen bleibt dort und ist nicht mehr am boden.

2.Positionieren Sie nun alle Elemente lediglich mit position: relative. Wodran
richten sich hierbei die Elemente aus? Ändert sich das Verhalten, wenn auch das Elternelement
(<div>) auch ein position:relative besitzt? Wie groß sind die Boxen bei
relativer Positionierung? Was passiert mit den nachfolgenden (Geschwister-)Elementen?
Was für Probleme treten bei welchen Elementen auf, wenn Sie versuchen das Wireframe
lediglich mit relativer Positionierung darzustellen?

Ohne left,right,top,bottom sind elemente unter ein ander. 
Die elemente orientieren sich an der Position, die das Element im Normalfall einnehmen würde.
Wenn div auch relative ist blibt alles gliech.
Die Boxen sind so groß, dass der Text in sie passt (header,nav und article). Aside, header und footer haben width 100% (trotzdem sind sie blocks)
Alle geschwister elemente sind zum Beispiel nach links, wenn div nach links ist.
Probleme sind mit aside. right:0 wirkt nicht, deshalb muss mann left:xxpx verwenden.

3.Positionieren Sie nun die Elemente mit einer Mischung aus relativer und absoluter Positionierung
möglichst genau, so dass das Aussehen wie im Wireframe erreicht wird. Was für
Probleme treten bei welchen Elementen auf?

Ohne left, right kann man die Elemente nicht richting stellen.
Wenn wir höhne von header andern müssen wir auch top von nav, article und aside ändern.

4.Setzen Sie beim <aside>-Element die Positionierung auf fixed. Wonach richtet sich
hierbei die Positionierung? Was passiert mit den nachfolgenden (Geschwister-)Elementen?

Wenn wir scrollen blieibt aside immer 5.6em unter top der Website. Die Geschwister-Elementen in aside bleiben wie sie waren.

5 Legen Sie nun den <article> und den <aside>-Block übereinander und vergeben Sie
unterschiedliche Hintergrundfarben mit background-color. Verwenden Sie z-Index2
um zu bestimmen, welche Fläche die andere überlagert. Erklären Sie die Funktionsweise
dieser Eigenschaft.

Element mit höher index in auf Element mit niedriger index.