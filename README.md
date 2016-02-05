
## ViewApp

### UIView, UIViewController och Interface Builder

Alla appar som innehåller någonting grafiskt (det vill säga alla appar) är uppbyggda av vyer och vy-kontroller. En vy (view) kan ses som en grafisk rityta. Den har en storlek, position och kan innehålla andra vyer samt egenutritad data. Alla färdiga komponenter, såsom knappar och textrutor, är i grund och botten vyer men är även utökad med mer funktionalitet. En vy-kontroller (view-controller) innehåller styrlogik som bestämmer vad vyn ska göra. Om vyn till exempel är en knapp så skulle styrlogiken (som då skulle ligga i en vy-kontroller) kunna vara koden som bestämmer vad som händer när användaren trycker på knappen.

Som uppmärksam läsare har du säkert redan listat ut att det är designmöntret Model-View-Controller (MVC) det rör sig om. Nästan all form av grafisk programmering som du gör när du utvecklar till iPhone eller iPad kretsar kring vyer och vy-kontroller. Du har redan stött på dessa i tidigare uppgifter, utan att kanske tänka så mycket på det. Hädanefter kommer dessa utgöra en stor del av den utveckling du gör, så ta dig tid och försök att verkligen sätta dig in i hur dessa fungerar och används.

Att som programmerare sitta och försöka lista ut exakt hur stor en viss komponent ska vara eller var den ska placeras är ett ganska omständigt och tråkigt arbete. För att göra detta enklare kan du med hjälp av storyboards designa ditt gränsnitt grafiskt (UI-designläget i XCode var tidigare en separat applikation som hette Interface Builder). Med Interface Builder kan du bygga grafiska gränssnitt enligt traditionella drag-och-släpp-metoder. För att få element att hamna på den plats man vill i runtime så måste man definera constraints och detta görs med auto layout.

### Förberedelser

#### Länkar

* Läsa
	* Guider 
		* [Auto layout guide][auto-layout-guide]
		* [Programming with Objective-C - Working with Blocks][working-with-blocks]
		* [Target-Action][target-action]
	* Dokumentation
		* [AlertViewController][alert-view-controller]
		* [UIView][uiview]
		* [UIViewController][uiview-controller]
* Screencasts
	* [Auto layout][auto-layout]
	* [Vykontroller][vykontroller]
	* [Vyer][vyer]


[vyer]:http://www.ida.liu.se/~725G72/material/screencasts/vyer.mp4

[vykontroller]:http://www.ida.liu.se/~725G72/material/screencasts/vykontroller.mp4

[auto-layout]:http://www.ida.liu.se/~725G72/material/screencasts/autolayout.mp4

[uiview]:https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIView_Class/

[uiview-controller]:https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIViewController_Class/

[alert-view-controller]: https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIAlertController_class/

[auto-layout-guide]:https://developer.apple.com/library/watchos/documentation/UserExperience/Conceptual/AutolayoutPG/Introduction/Introduction.html

[target-action]:https://developer.apple.com/library/ios/documentation/General/Conceptual/Devpedia-CocoaApp/TargetAction.html

[working-with-blocks]:https://developer.apple.com/library/ios/documentation/Cocoa/Conceptual/ProgrammingWithObjectiveC/WorkingwithBlocks/WorkingwithBlocks.html

#### Förberedelseuppgifter / frågor

Inga frågor är märkta för att redovisas till denna uppgift.

1. Förklara skillnaden mellan begreppen "frame" och "bounds" för en vy.
2. Hur gör man för att skapa en ny vy? Skriv kod som skapar en vy på position (100, 150) med bredden 80 och höjden 90 samt lägger till den som sub-vy till foobar (antag att foobar är en variabel av typen UIView).
3. För att koppla samman komponenter i en storyboard och koden används nyckelordet IBOutlet. Hur används IBOutlet? Betyder nyckelordet någonting speciellt i koden? Hur gör du för att koppla en vy till en property i koden? Vilka attribut bör propertyn ha? Ge exempel på hur en sådan property kan se ut.
4. En vy-kontroller har en stark referens till sin huvudvy (view propertyn). Placerar man en knapp i den vyn och vill koppla knappen till koden ska den kopplas med en svag referens. Förklara skillnaden utifrån minneshantering.
5. På samma sätt som du kopplar samman en vy med en property så kopplar du ihop händelser med metoder, så att till exempel en viss metod anropas när en knapp trycks ned. För att göra detta i Interface Builder används nyckelordet IBAction. Hur används IBAction? Betyder nyckelordet någonting? Hur gör du sammankopplingen mellan en händelse och en metod? Beskriv hur du gör både via Interface Builder och i kod. Vilken händelse används vanligen för ett vanligt tryck på skärmen?
6. Vilken metod i UIViewController använder du i allmänhet för att initiera egna variabler och data?

### Uppgift

I det färdiga programmet ska du öva på att använda Interface Builder för att bygga gränssnitt. Du kommer även att få testa på att använda dig av block. Det finns en del given kod men en hel del ska du komplettera med själv.

Innan du börjar skriva någon kod eller ändrar på någonting, läs noga igenom alla kommentarer i koden. Exakt vad som ska göras finns väl kommenterat där. Uppgiften är uppdelad i två olika delar. Börja med FirstViewController och fortsätt i stigande ordning.

[ViewApp](https://github.com/Linkopings-Universitet/ViewApp)

### Redovisning

Packa ihop det modifierade projektet och skicka fil och svaren på förberedelseuppgifterna till din handledare. Ange '725G72 - Laboration 3 - Redovisning' som ämne. Skriv med vad du har för LiU-id (t ex abcde123) om du inte mailar från din studentadress.