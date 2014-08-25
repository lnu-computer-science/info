Denna handledning innehåller en introduktion till git och github samt en förklaring till varför vi vill att du använder github i undervisningen. 
Du kommer också i denna handledning få en introduktion till hur du börjar arbeta med Git för att kunna använda det i de kurser du kommer gå.
Observera dock att enskilda kurser kan ha olika krav på hur man ska använda github men det framgår i så fall av respektive kurs webbplats.

För att hänga med i guiden utgår vi från att du har en grundläggande datorkunskap.

Har du tidigare arbetat med git/github kan du mycket väl ha invanda arbetssätt som du är fri att använda även i våra kurser, men läs igenom guiden nedan så du får en bild av vilka speciella krav vi ställer. 


Vad är git och github?
---------

[git](http://git-scm.com/ "Den officella sidan om git") är ett versionhanteringssytem som är utarbetat främst för muukvaruutvecklare och hantering av kod. Med ett [versionshanteringssystem](http://sv.wikipedia.org/wiki/Versionshantering) menas att systemet hjälper användaren att hantera filer och spara dem i olika versioner så att man kan spåra förändringar och gå tillbaka i historiken. Det ger också möjligheter för flera utvecklare att kunna samarbeta kring samma filer utan att riskera att man skriver över någon annans arbete. Du kommer under din utbildning att använda dig mycket av Git men även andra versionhanteringssytem så som t.ex. subversion (svn). [Mer information om versionshantering](http://git-scm.com/book/en/Getting-Started-About-Version-Control).

Git skapades av [Linus Torvalls](http://sv.wikipedia.org/wiki/Linus_Torvalds "Linus Torvalds wikipedia"), ett namn som säkert många känner till som skaparen till operativsystemet Linux. [Git uppkom](http://git-scm.com/book/en/Getting-Started-A-Short-History-of-Git) helt enkelt för att Linus inte tyckte att det fanns ett bra och fritt versionhanteringssystem som kunde hantera all kod som Linux består av och underlätta för alla de olika utvecklare som är inblandade i utvecklingen av Linux. 

I många av våra kurser kommer vi också använda tjänsten [Github](http://github.com/ "Githubs hemsida"). Github är en tjänst som ger oss utvecklare möjlighet att, via webben, skapa, hantera och lagra projekt och dess via Git. Github ger oss också möjlighet att dela kod med andra, studera andras kod och använda andras kod för att bygga vidare på. Github är alltså en tjänst för "social coding". Man kan också använda github för att dela utvecklingsfiler i privata grupper eller som ensam utvecklare hantera sina filer på ett smidigt sätt. Vi skulle kunna kalla det ett slags Facebook, fast för kod. På senare tid har dock allt fler upptäckt möjligheterna med Git och Github och nu för tiden hittar man inte bara mjukvaruprojekt på Github.


Varför vill vi att du använder Git och Github?
---

I många av våra kurser kommer det vara krav på att använda Git och Github för att hantera kod och dokumentation. Detta beror på flera saker:

* Först och främst kommer Git och Github vara något du med säkerhet kommer stöta på i ditt kommande arbetsliv.
* Ditt Github-konto kommer fungera som ett CV där du samlar din kod och där eventuella arbetsgivare kan se vad du kan och har producerat tidigare. Dett aär något vi märker fler och fler arbetsgivare nämner så att redan från början bygga upp sitt Githubkonto bör vara en viktig punkt i din utveckling.
* Du kommer enklare kunna hantera dina filer. Inga datorkrasher kommer få dina filer att försvinna, du kan komma åt dina filer från flera olika datorer och enheter.
* Du kan enkelt dela dina filer med dina lärare. Vid examinering av t.ex. koduppgifter vill läraren titta på din kod och kan då via github enkelt komma åt denna. Vid t.ex. frågor kring eller problem med din kod kan läraren enkelt komma åt den senaste versionen.
* I vissa kurser kommer ni att arbeta i grupper och github ger en bra möjlighet att sammarbeta kring kodfilerna.
* Github är ett kraftfullt verktyg för att studera och lära sig av andras kod.
* Läraren kan följa dina versioner och se hur du ligger till i kursen.
* Github har också ett system för att skriva kommentarer, ToDo-listor m.m som underlättar vid utvecklandet.


Att börja använda Git
---
Vi ska börja titta på hur vi arbetar med Git. Denna guide har valt att koncentrera sig på hur man arbetar med Git via en kommandotolk/ett terminalfönster. Det finns grafiska klienter att använda men dessa får du själv upptäcka när du väl lärt dig grunderna i Git-kommandon. Du kommer arbeta med kommandotolken/terminalfönstret mycket under din utbildning så att bli van vid att arbeta via den är också viktigt.

## Installera Git på din dator
Om du arbetar på en egen dator är det en bra start att börja med att installera Git. Använder du skolans datorer bör det redan vara installerat på dessa. Att installera Git är inte svårare än att installera något annat program. Du laddar ner och installerar en körbar fil. [Mer information hittar du på Git:s officiella sida](http://git-scm.com/book/en/Getting-Started-Installing-Git). Välj sätt att installera på beroende på ditt operativsystem.

## Konfigurera Git
För att på ett enkelt sätt komma igång kan vi börja med att konfiguera Git genom att tala om vem vi är.

### *Mac*
Öppna terminalfönstret genom att söka upp det i "Spotlight" (programmet heter Terminal) eller via finder "Go" --> "Utilities" --> "Terminal".

BILD HÄR!

### *Windows*
Du öppnar ett terminalfönster i Windows genom att du går via startmeny --> "Git" --> "Git bash".

### De första inställningarna
Börja med att testa att din installation är korreckt genom att skriva:
*git --version*
Du bör då få upp en bild liknande denna:

BILD HÄR

Forsätt genom att ange dina uppgifter i konfigurationen för Git. Använd såklart ditt namn och e-postadress (din studentadress)
*git config --global user.name "John Doe"*
*git config --global user.email johndoe@example.com*

Kontrollera dina inställningar via:
*git config --list*

# Att skapa ett repositorie
Ett centralt begrepp inom Git är repositorie (repository) eller ofta förkortat som repo. Detta kan förklaras som ett versionshanterat projekt. Vi kan likna ett repositorie med en mapp/katalog innehållandes filer och undermappar som kan versionshanteras. Du skapar oftast ett repositorie per kurs eller per applikation.

Ett repositorie kan skapa på olika sätt. Antingen via att skapa ett helt nytt repo på din lokala dator eller genom att ladda ner ett redan påbörjat repo från t.ex. Github,

## Skapa ett nytt lokalt repositorie
Börja med att använda kommandot cd i terminalen för att bege dig till någon lämplig katalog där du vill skapa ditt repositorie. Väl där skapar du en ny mapp genom att skriva:

mkdir my_application 

Detta skapar en katalog med namnet my_application. För att skapa ett repositorie i denna mapp navigerar du dig in i mappen och där skriver "git init".

SE BILD

Du har nu skapat ett helt eget lokalt repositorie och har förmodligen fått en mapp som heter ".git" (kan vara dold i mac). Den mappen innehåller all information om detta repositorie och de versionsförändringar vi kommer göra. Denna mapp ska du alltså inte bry dig om så mycket utan bara låta Git sköta om.

Du kan nu testa status på ditt repo genom att skriva
*git status*

Än har vi ju inte lagt till några filer i vår versionshanterade katalog (vårt repo). Så skapa en fil index.html i valfri editor och spara i katalogen du nyss skapade. Kontrollera nu statusen med *git status* och observera nu skillnaden.

BILD HÄR

Git har alltså upptäckt att vi lagt till en ny fil i mappen och talar om att denna inte är versionshanterad. Varje fil i en mapp som är Git-hanterad kan antingen vara "tracked" eller "untracked". För att lägga till filen index.html vi nyss skapade skriver du:
*git add index.html*
Ovanstående kommando lägger till just filen index.html. Har man skapat flera filer samtidigt som vill lägga till använder man:
_git add *_ 
Vilket också är det man brukar använda i nästan alla fall.
Kolla nu status på ditt repositorie igen med *git status*

Filen är nu tillagd men den är fortfarande inte versionshanterad. Vi måst egöra en så kallad "commit" för att få detta. En "Commit" gör man när man suttit och jobbat ett tag med någon ting, kanske skrivit en deluppgift, implementerat en funktion i sin applikation eller kanske bara tar en paus och vill "checka in" det man gjort hittils. Man brukar säga att man ska "commit:a" sin kod ofta men inte så att det blir svårt att följa utvecklingen av projektet. En "Commit" ska också innehålla en br akommentar som beskriver för andra vad du gjort sedan sist. Även om du komemr jobba ensam i vissa repositorier så var noga med att skriva bra och förklarande kommentarer till dina commits. För att göra en commit skriver du:

*git commit -m "Jag har precis skapat filen index.html. Den är dock fortfarande tom"*

Du bör såklart byta ut kommentaren innanför citattecknen mot en kommentar som passar i ditt fall, Kontrollera nu ditt repositories status

BILD HÄR

Testa nu att göra en ändring i filen index.html samt skapa en ny fil och lägg i mappen. Kolla status, lägg till den nya filen med *git add* och gör en ny commit.

Du bör nu ha ett lokalt repositorie med två versionshanterade filer och två styckens "commits".

## Skapa ett repositorie på github och klona ner lokalt






Hur börjar man med github?
---
När man som ovan börjar jobba med git och github kommer man stöta på vissa ord som kan vara viktiga att känna till. Vanliga ord som vi kommer använda är:

* Repositorie - "repo" är oftast ett projekt. Vi kan likna ett repositorie med en mapp/katalog innehållandes filer och undermappar som kan versionshanteras. Du skapar oftast ett repositorie per kurs.
* Commit - Att "commita" sina ändringar talar om att man nu har uppdaterat sina filer och sparar dessa i en ny version, en commit.
* Forking - Detta innebär att man hittar ett intressant projekt som någon annan lagt ut och som man själv vill bygga vidare på. "Forkar" man då projektet får man en kopia av alla filer som man kan fortsätta jobba vidare med på egen hand.
* Pull request - Detta innebär att du har forkat ett projekt/repositorie och gjort förändringar i detta som du vill dela med dig av till orginalprojketet. Du kan då föreslå detta för repositorie-ägaren genom att göra en "pull request" som ägaren får godkänna.
* Merge - Om ägaren av repositoriet tycker att dina ändringar är bra kan hon/han välja att baka in dessa i orginalkoden d.v.s. göra en "merge", en sammanslagning.
* Branch/Branching - Du kommer att använda "branching" eller förgreningar i ditt repro för att undvika att ändra i projektets huvudgren. Detta är extra viktigt då man är flera personer som samarbetar i samma repro.

Här är några fler resurser kring git och github:
[Introduction to Git with Scott Chacon of GitHub](http://www.youtube.com/watch?v=ZDR433b0HJY "Youtubevideo om git")


Det första Du bör göra är att [skapa dig ett konto på github](http://www.github.com). Här är det viktigt att du __registrar dig med din studentmejl från LNU__. Detta för att du ska kunna registrera ett education-konto och på så sätt kunna skapa vad man kallar privata repositorier, alltså kodprojekt som ingen annan än du och de du väljer att samarbeta med kan se. Välj gärna ett användarnamn som innehåller ditt användarnamn här på LNU.

![Skapa ett konto på github][github_reg] 

Fyll i formuläret som ovan fast med ditt eget användarnamn.




Uppgradera ditt github-konto till education
---------------------------------------------
![Skapa ett educationkonto på github][github_reg_edu] 
Nästa steg är att registrera detta nyskapade konto som ett studentkonto. Gå till länken: [http://www.github.com/edu](http://www.github.com/edu)
Välj **Request a discount**, logga in om du inte gjort det och välj sedan **Student**, klicka på nästa och följ instruktionerna. Efter denna process bör du få ett e-postmeddelande från github och du har möjlighet att skapa privata så kallade repositorier. Oftast kommer du använda ett repositorie per kurs.


Skapa ett repositorie
-----------------------
Nu är det dags att skapa ditt första repositorie. Det gör du från din startsida på github när du loggat in.

<img src="https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_startpage.png" width="80%" />

Klicka på knappen "new repository" och fyll i dina uppgifter. Går du en kurs har du säkert fått information om vad du ska döpa detta repositorie till.

![Githubs - skapa ett nytt repositorie][github_repo_new] 
Du kan här välja om du vill skapa ditt repositorie public (alla kan se din kod) eller private. Bara du och de du delar ditt repositorie med kan se dina filer. Beroende på kurs så kan det vara olika krav på om koden får vara publik eller privat. 


Dela ditt repositorie *(OBS, kan skilja sig från kurs till kurs)*
----------------------
Ska du använda ditt repositorie i en kurs är det troligt att du ska dela det med din lärares kurskonto. Möjligheten till att dela ditt hittar du genom att klicka på
ikonen med verktyg (settings) till höger på sidan.

![Inställningar i github][github_settings] 

Välj sedan "Collaborators" och skriv in namnet på det kontot/användarnamnet du vill dela ditt repositorie med:

![Collaborators][github_collaborator] 


Att börja jobba med ditt repositorie 
-------------------------------------
Nu bör du vara registrerad på github med ett education-konto och du kan egentligen börja använda github för att hantera dina filer i dina kurser. Detta kan skilja sig lite åt från kurs till kurs med hur du gör bör där framgå av kurshemsidan.

Föreslå förändringar på denna handledning
------------------------------------------
Detta dokument ligger på [github](https://github.com/LNU-CoursePress/info/blob/master/manualer/github_start.md) och hittar du felaktigheter eller vill föreslå förändringar går det bra att göra det där.

Referenser
-----------

* [Pro Git](http://git-scm.com/book) - Fri e-bok som är fullmatad med nyttig information kring Git.

[github_reg]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_register.png "Github registration"
[github_reg_edu]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_register_edu.png "Github registration education"
[github_startpage]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_startpage.png "Github startpage"
[github_repo_new]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_repo_new.png "New repository"
[github_settings]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_settings.png "Settings"
[github_collaborator]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_collaborator.png "github_collaborator"
