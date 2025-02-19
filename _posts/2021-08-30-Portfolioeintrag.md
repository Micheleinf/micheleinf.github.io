---
layout: post
title: Portfolioeintrag 133
---

# Wie man Benutzereingaben in XHTML speichert
Die ist der Portfolioeintrag für das Modul 133
## Aufgabenstellung
Im Modul 133 geht es darum responsive Web-Seiten mit XHTML zu erstellen. In diesem Blog will ich zeigen, wie man mit Beans in XHTML Benutzereingaben speichert. Programmiert wurde in NetBeans IDE 12.0

**Ziele**
- Verstehen wie Beans funktioniert
- Benutzereingaben speichern
- Benutzereingabe ausgeben

## Produkt
Wir haben ein `eyecolor.xhtml` um die Augen Farben eines Benutzers zu speichern der Code dazu sieht wie folgt aus:
```xml
<h:form id="eyecolor-form">  
<h:outputLabel for="eyecolor">Eyecolor</h:outputLabel>  
<h:inputText id="eyecolor" value="#{character.eyecolor}" required="true" requiredMessage="A eyecolor is required"/><br/>  
```
Die Eingabe wollen wir dann in einem anderen formular/site ausgeben, dazu adden wir folgenden code:
```xml
<h:commandButton id="submit-button" value="Submit" action="final.xhtml"/>  
```
So sieht das aus für den Benutzer:


![eyeui](https://user-images.githubusercontent.com/54061875/131363269-d08313c5-2644-4d2a-b1ec-356cdabe7fde.PNG)


Dadurch wird beim Ausfüllen und abschicken des Formulars eine neue Seite aufgerufen die ich `final.xhtml` benannte und folgenden code gab:
```xml
<h:outputText value="Deine Augenfarbe: #{character.eyecolor}"/>
```
Dadurch haben wir eine Benutzereingabe gespeichert und wieder herausgegeben.




## Reflexion und Zerfifizierung
Diese Aufgabe zu erstellen ging ganz gut und war nicht allzu schwierig mit der Erklärung der Präsentationen und dem Input unserem Lehrmeister war es ganz einfach das Speichern und Ausgeben von Benutzereingaben in XHTML zu erstellen/coden. Eine Verbesserung könnte gemacht werden bei der Benutzereingabe anstatt ein Label ein Dropdown mit den verschiedenen Augenfarben, um Fehlereingaben zu vermeiden.

- Verstehen wie Beans funktioniert ✔️
*Ich habe verstanden wie Beans mir bei Benutzereingaben weiter hilft und kann dies jetzt umsetzen*
- Benutzereingaben speichern ✔️
*Wurde umgesetzt, siehe dabei den Code bei Produkt*
- Benutzereingabe ausgeben ✔️
*Wurde umgesetzt, siehe dabei den Code bei Produkt*
































