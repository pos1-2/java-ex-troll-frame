Übung 7 - Trollfenster
===================


1 Zufällige Buttonposition
-------------

Beim Programmstart wird ein `JFrame`mit einem einzigen `JButton` darauf erzeugt und angezeigt.

Der Button soll mit `"Schließen"` beschriftet sein, aber keine Funktion haben.

Die Position des Buttons soll zufällig festgelegt sein. Achten Sie aber darauf, dass er `JButton` immer vollständig sichtbar ist! (Also nicht über den Fensterrand hinausragt, oder gar gänzlich außerhalb des `JFrame` liegt).

`getBounds`, `setLocation`, [`JFrame` Größe ermitteln](JFRAME-SIZE.md)

2 Flüchtiger Button
-------
Wenn man mit der Maus über den `JButton` fährt (z.B. um diesen zu drücken), soll der `JButton` seine Position so verändern, dass er nicht mehr unter dem Mauszeiger liegt (aber noch immer sichtbar innerhalb des Fensters).

Verwenden Sie dazu die Funktionalität aus Punkt 1 wieder: Setzen Sie die Position des `JButtons` einfach erneut zufällig - Sollte der `JButton` (zufällig) schon wieder unter dem Mauszeiger erscheinen, wiederholen sie den Prozess einfach.

`JButton.addMouseListener`, `MouseAdapter`, `MouseListener.mouseEntered`, `MouseEvent.getPoint` oder `MouseEvent.getLocationOnScreen`, `SwingUtilities.convertMouseEvent` oder `SwingUtilities.convertPointFromScreen`

3 Hydra X Knopferl
------
Wenn man das X Knopferl in der oberen Fensterecke drückt, soll anstatt, dass sich das `JFrame` schließt, das `JFrame` verdoppeln.

`JFrame.setDefaultCloseOperation(WindowConstants.DO_NOTHING_ON_CLOSE)`,
`JFrame.addWindowListener`, `WindowAdapter`, `WindowListener.windowClosing`

4 Geheimausgang
----
Denken Sie sich ein Passwort aus, wenn man das Passwort auf der Tastatur eingibt, während das `JFrame` geöffnet und das aktuelle Fenster ist, dann soll sich die Applikation beenden.

`addKeyListener`, `KeyAdapter`, `KeyListener.keyTyped`, `KeyEvent.getKeyChar`,
`System.exit`

5 Paketieren
-----
Packen Sie Ihr Programm in eine ausführbare `.jar` dabei, damit Sie Ihren Bekannten zeigen können, was Sie alles tolles in der Schule lernen.

Siehe Anleitung hier: http://stackoverflow.com/a/5293338
