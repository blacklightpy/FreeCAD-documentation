---
- GuiCommand:/es
   Name:Part Plane
   Name/es:Part Plano
   MenuLocation:Pieza → Crear primitivas... →Plano
   |Workbenches:[Part](Part_Workbench/es.md)
   SeeAlso:[Part Primitivas](Part_Primitives/es.md)
---

# Part Plane/es


</div>

## Description


<div class="mw-translate-fuzzy">

## Descripción

Crea un Plano paramétrico simple de 10 x 10 mm, con los parámetros de posición, longitud y anchura. Por defecto, el Plano es colocado en el origen (0,0,0).


</div>

<img alt="" src=images/Part_Plane_Example.png  style="width:400px;">

## Uso

See [Part Primitives](Part_Primitives#Usage.md).

## Example

![Part Plane from the scripting example](images/Part_Plane_Scripting_Example.png )

A Part Plane object created with the [scripting example](#Scripting.md) below is shown here.

## Properties

See also: [Property editor](Property_editor.md).

A Part Plane object is derived from a [Part Feature](Part_Feature.md) object and inherits all its properties. It also has the following additional properties:

### Data


{{TitleProperty|Attachment}}

The object has the same attachment properties as a [Part Part2DObject](Part_Part2DObject#Data.md).


{{TitleProperty|Plane}}

-    **Length|Length**: The length of the plane. This is the dimension in its X direction. The default is {{Value|10mm}}.

-    **Width|Length**: The width of the plane. This is the dimension in its Y direction. The default is {{Value|10mm}}.

## Scripting

See also: [Autogenerated API documentation](https://freecad.github.io/SourceDoc/), [Part scripting](Part_scripting.md) and [FreeCAD Scripting Basics](FreeCAD_Scripting_Basics.md).

A Part Plane can be created with the {{Incode|addObject()}} method of the document:


```python
plane = FreeCAD.ActiveDocument.addObject("Part::Plane", "myPlane")
```

-   Where {{Incode|"myPlane"}} is the name for the object.
-   The function returns the newly created object.

Example:


```python
import FreeCAD as App

doc = App.activeDocument()

plane = doc.addObject("Part::Plane", "myPlane")
plane.Length = 4
plane.Width = 8
plane.Placement = App.Placement(App.Vector(1, 2, 3), App.Rotation(20, 75, 60))

doc.recompute()
```





{{Part_Tools_navi

}}



---
![](images/Right_arrow.png) [documentation index](../README.md) > [Part](Part_Workbench.md) > Part Plane/es
