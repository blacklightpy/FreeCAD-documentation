# Download/de
{{TOCright}}



## Aktuelle stabile Version 


<div class="mw-translate-fuzzy">

Die Version 0.20.1 von FreeCAD (29410) wurde am 10.08.2022 veröffentlicht. Um herauszufinden, was es Neues gibt, sIehe die [Veröffentlichungshinweise](Release_notes_0.20/de.md).


</div>


<div class="mw-translate-fuzzy">

SHA256 Prüfsummen zur Überprüfung der Integrität eines Downloads kann man auf der [0.20.1 Release-Page](https://github.com/FreeCAD/FreeCAD/releases/tag/0.20.1).


</div>

Frühere Versionen können von der Seite der veröffentlichten [Versionen](https://github.com/FreeCAD/FreeCAD/releases) heruntergeladen werden.

+::+::+::+
| ![](images/Windows.png )                                                                                         | ![](images/Mac.png )                                                                                                             | ![](images/Linux_with_text.png )     |
|                                                                                                                        |                                                                                                                                    |                                                    |
| [Install on Windows](Installing_on_Windows.md)                                                                 | [Install on Mac](Installing_on_Mac.md)                                                                                     | [Install on Linux](Installing_on_Linux.md) |
|                                                                                                                        |                                                                                                                                    |                                                    |
| [64-bit installer](https://github.com/FreeCAD/FreeCAD/releases/download/0.20.2/FreeCAD-0.20.2-WIN-x64-installer-2.exe) | [macOS 64-bit](https://github.com/FreeCAD/FreeCAD/releases/download/0.20.2/FreeCAD_0.20.2-2022-12-27-conda-macOS-x86_64-py310.dmg) | [AppImage 64-bit](AppImage.md)             |
++++

### Hinweise für Windowsbenutzer 

-   Die folgenden Windows Versionen werden unterstützt: 64-bit 7/8/10/11. 32-bit-Windows wird nicht unterstützt.
-   Eine portable Version, die keine Installation benötigt, steht unter [Veröffentlichungen](https://github.com/FreeCAD/FreeCAD/releases/) zur Verfügung.
-   Das Paket kann auch vom [Chocolatey](https://chocolatey.org/packages/freecad)-Manager installiert werden.


<div class="mw-translate-fuzzy">

### Hinweise für Mac OS X Benutzer 

Mac OS X 10.12 Sierra ist die minimal unterstützte Version.


</div>



### Hinweise für GNU/Linux Anwender 

Die meisten Distributionen führen FreeCAD in ihren offiziellen Repositorien, aber wenn die Distribution nicht einem rollierenden Veröffentlichungs Modell folgt, kann die von ihnen bereitgestellte Version veraltet sein. Stattdessen kannst Du das AppImage oben herunterladen, als ausführbar markieren und ohne Installation starten.

Bitte schau auf der Seite [Installation unter Linux](Installing_on_Linux/de.md) nach weiteren Installationsoptionen, einschließlich täglicher Pakete für Ubuntu und Derivaten.

Eine portable Version, welche keine Installation benötigt, kann durch Starten von FreeCad mit diesen Befehlen erreicht werden:


{{Code|lang=text|code=
cd path/to/directory_containing_AppImage/
chmod +x ./name_of_AppImage_file.AppImage
HOME="$PWD/Settings" FREECAD_USER_HOME="$PWD/Settings" ./name_of_AppImage_file.AppImage
}}

Weitere Informationen über die Umgebungsvariablen von FreeCAD können auf der [Konfigurationsseite](Start_up_and_Configuration/de#Environment_variables.md) gefunden werden.


<div class="mw-translate-fuzzy">

## Entwicklungsversionen

Die Entwicklung von FreeCAD ist aktiv.

-   Für Linux Anwender probiere die Entwicklung [AppImage](AppImage/de.md) aus.
-   Für MacOS und Windows Entwicklungsbuilds und Entwicklungsquellcode siehe die [weekly builds](https://github.com/FreeCAD/FreeCAD-AppImage/releases/tag/weekly-builds) Seite.
-   Um den neuesten Quellcode zu kompilieren, siehe [Kompilieren](Compiling/de.md).


</div>



## Zusätzliche Module und Makros 


<div class="mw-translate-fuzzy">

Die FreeCAD Gemeinschaft bietet viele zusätzliche Module und Makros. Seit 0.17 können sie einfach aus FreeCAD heraus mit dem [Addon-Manager](Std_AddonMgr/de.md) installiert werden <img alt="" src=images/Std_AddonMgr.svg  style="width:24px;">.


</div>



---
![](images/Right_arrow.png) [documentation index](../README.md) > Download/de
