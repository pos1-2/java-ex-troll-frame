
Wie bekomme ich die tatsächliche Größe von dem Inneren des ```JFrame```
=====================

1. Wunschgröße äußern
```
// "ich haette gern diese groesse"
frame.getContentPane().setPreferredSize(new Dimension(width, height)); 
```

2. Swing Magie aktivieren
```
// das fenster legt seine groesse selbstständig fest, versucht ihre wünsche dabei zu erfüllen
frame.pack(); 
```

3. Tatsächliche Größe erfragen
```
frame.getContentPane().getSize() 
// liefert jetzt die tatsächliche grösse vom inneren bereich
```
