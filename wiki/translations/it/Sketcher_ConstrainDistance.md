---
- GuiCommand:/it
   Name:Sketcher ConstrainDistance
   Name/it:Distanza
   Workbenches:[Schizzo](Sketcher_Workbench/it.md)
   MenuLocation:Sketch → Vincolo → Distanza
   Shortcut:**Maiusc** + **D**
   SeeAlso:[Distanza Orizzontale](Sketcher_ConstrainDistanceX/it.md), [Distanza Verticale](Sketcher_ConstrainDistanceY/it.md)
---

# Sketcher ConstrainDistance/it


</div>

## Description


<div class="mw-translate-fuzzy">

## Descrizione

Il vincolo **Distanza** impone alla lunghezza di una linea, alla distanza perpendicolare tra un punto e una linea o alla distanza tra due punti di assumere un valore specifico.


</div>

![](images/Sketcher_ConstrainDistance_example.png )

## Utilizzo


<div class="mw-translate-fuzzy">

1.  Selezionare due punti o una linea
2.  Richiamare il comando in uno di questi modi:
    -   Cliccare sull\'icona **[<img src=images/Sketcher_ConstrainDistance.png style="width:24px"> '''Distanza'''** della barra degli strumenti.
    -   Usare la scorciatoia da tastiera **Maiusc** + **D**.
    -   Usare la voce **Sketch → Vincoli → Distanza** dal menu principale.
3.  Si apre una finestra di dialogo per modificare o confermare il valore. Premere **OK** per confermare.


</div>


<div class="mw-translate-fuzzy">

**Nota:** lo strumento di vincolo può essere avviato anche senza selezione precedente. Per impostare la distanza perpendicolare tra un punto e una linea, il punto deve essere selezionato per primo. Di default il comando è in modalità continua per creare nuovi vincoli; per uscire dal comando premere il tasto destro del mouse o una volta il tasto **ESC**.


</div>

### Hint


<div class="mw-translate-fuzzy">

### Suggerimento

Quando sono applicabili conviene usare il vincolo **[<img src=images/Sketcher_ConstrainDistanceX.svg style="width:16px"> [Distanza Orizzontale](Sketcher_ConstrainDistanceX/it.md)** o il vincolo **[<img src=images/Sketcher_ConstrainDistanceY.svg style="width:16px"> [Distanza Verticale](Sketcher_ConstrainDistanceY/it.md)**. Questi vincoli sono più robusti e più veloci da calcolare rispetto al vincolo di Lunghezza documentato qui.


</div>

## Scripting

Distance from origin:


```pythonSketch.addConstraint(Sketcher.Constraint('DistanceX', Edge, PointOfEdge, App.Units.Quantity('123.0 mm')))```

Distance between two vertices:


```pythonSketch.addConstraint(Sketcher.Constraint('Distance', Edge1, PointOfEdge1, Edge2, PointOfEdge2, App.Units.Quantity('123.0 mm')))```

Length of line (the GUI allows selecting the edge itself, but it is just a shorthand for using the two extremities of the same line):


```pythonSketch.addConstraint(Sketcher.Constraint('Distance', Line, 1, Line, 2, App.Units.Quantity('123.0 mm')))```

Distance from point (`Edge, PointOfEdge`) to nearest point on line (`Line`):


```pythonSketch.addConstraint(Sketcher.Constraint('Distance', Edge, PointOfEdge, Line, App.Units.Quantity('123.0 mm')))```

The [Sketcher scripting](Sketcher_scripting.md) page explains the values which can be used for `Edge1`, `Edge2`, `Edge`, `PointOfEdge1`, `PointOfEdge2`, `PointOfEdge` and `Line`, and contains further examples on how to create constraints from Python scripts.


<div class="mw-translate-fuzzy">





</div>


{{Sketcher_Tools_navi

}}



---
![](images/Right_arrow.png) [documentation index](../README.md) > [Sketcher](Sketcher_Workbench.md) > Sketcher ConstrainDistance/it
