Denna handledning innehåller en introduktion till git och github samt en förklaring till varför vi vill att du använder github i undervisningen. Observera dock att enskilda kurser kan ha olika krav på hur man ska använda github men det framgår av respektive kurs webbplats.

För att hänga med i guiden krävs grundläggande datorkunskap.

Har du tidigare arbetat med git/github kan du mycket väl ha invanda arbetssätt som du är fri att använda även i våra kurser, men läs igenom guiden nedan så du får en bild av vilka speciella krav vi ställer. Guiden är förenklad för att passa nybörjare.

Vad är git och github?
---------

[git](http://git-scm.com/ "Den officella sidan om git") är ett versionhanteringssytem som är utarbetat främst för utvecklare och hantering av kod. Med ett [versionshanteringssystem](http://sv.wikipedia.org/wiki/Versionshantering) menas att systemet hjälper användaren att hantera filer och spara dem i olika versioner så att man kan spåra förändringar och gå tillbaka i historiken. Det ger också möjligheter för flera utvecklare att kunna samarbeta kring samma filer utan att riskera att man skriver över någon annans arbete. 

Du kommer under din utbildning att använda dig av git men även andra versionhanteringssytem så som t.ex. subversion (svn).
Git skapades av [Linus Torvalls](http://sv.wikipedia.org/wiki/Linus_Torvalds "Linus Torvalds wikipedia"), ett namn som säkert många känner till som skaparen till operativsystemet Linux. [Git uppkom](http://git-scm.com/book/en/Getting-Started-A-Short-History-of-Git) helt enkelt för att Linus inte tyckte att det fanns ett bra och fritt versionhanteringssystem som kunde hantera all kod som Linux består av och alla de olika utvecklare som är inblandade i utvecklingen av Linux. 

I många av våra kurser kommer vi använda tjänsten [github](http://github.com/ "Githubs hemsida"). Github är en tjänst som ger oss utvecklare möjlighet att, via webben, skapa, hantera och lagra projekt via git. Github ger oss också möjlighet att dela kod med andra, studera andras kod och använda andras kod för att bygga vidare på. Github är alltså en tjänst för "social coding". Man kan också använda github för att dela utvecklingsfiler i privata grupper eller som ensam utvecklare hantera sina filer på ett smidigt sätt.

När man som ovan börjar jobba med git och github kommer man stöta på vissa ord som kan vara viktiga att känna till. Vanliga ord som vi kommer använda är:

* Repositories - "repos" är oftast ett projekt. Vi kan likna ett repositorie med en mapp/katalog innehållandes filer och undermappar som kan versionshanteras. Du skapar oftast ett repositorie per kurs.
* Commit - Att "commita" sina ändringar talar om att man nu har uppdaterat sina filer och sparar dessa i en ny version, en commit.
* Forking - Detta innebär att man hittar ett intressant projekt som någon annan lagt ut och som man själv vill bygga vidare på. "Forkar" man då projektet får man en kopia av alla filer som man kan fortsätta jobba vidare med på egen hand.
* Pull request - Detta innebär att du har forkat ett projekt/repositorie och gjort förändringar i detta som du vill dela med dig av till orginalprojketet. Du kan då föreslå detta för repositorie-ägaren genom att göra en "pull request" som ägaren får godkänna.
* Merge - Om ägaren av repositoriet tycker att dina ändringar är bra kan hon/han välja att baka in dessa i orginalkoden d.v.s. göra en "merge", en sammanslagning.

Här är några fler resurser kring git och github:
[Introduction to Git with Scott Chacon of GitHub](http://www.youtube.com/watch?v=ZDR433b0HJY "Youtubevideo om git")

Varför vill vi att du använder github?
---

I många av våra kurser kommer det vara krav på att använda github för att hantera sina kodfiler. Detta beror på flera saker:

* Först och främst kommer git och github vara något du med säkerhet kommer stöta på i ditt kommande arbetsliv och många arbetsgivare kan se det som en merit att ha erfarenhet av detta.
* Du kommer enklare kunna hantera dina filer. Inga datorkrasher kommer få dina filer att försvinna, du kan komma åt dina filer från flera olika datorer och enheter.
* Du kan enkelt dela dina filer med dina lärare. Vid examinering av t.ex. koduppgifter vill läraren titta på din kod och kan då via github enkelt komma åt denna. Vid t.ex. frågor kring eller problem med din kod kan läraren enkelt komma åt den senaste versionen.
* I vissa kurser kommer ni att arbeta i grupper och github ger en bra möjlighet att sammarbeta kring kodfilerna.
* Github är ett kraftfullt verktyg för att studera och lära sig av andras kod.
* Läraren kan följa dina versioner och se hur du ligger till i kursen.


Hur börjar man med github?
---
Det första Du bör göra är att [skapa dig ett konto på github](http://www.github.com). Här är det viktigt att du __registrar dig med din studentmejl från LNU__. Detta för att du ska kunna registrera ett education-konto och på så sätt kunna skapa vad man kallar privata repositorier, alltså kodprojekt som ingen annan än du och de du väljer att samarbeta med kan se. Välj gärna ett användarnamn som innehåller ditt användarnamn här på LNU.

![Skapa ett konto på github][github_reg] 

Fyll i formuläret som ovan fast med ditt eget användarnamn.

![Skapa ett educationkonto på github][github_reg_edu] 


Uppgradera ditt github-konto till education
---------------------------------------------
Nästa steg är att registrera detta nyskapade konto som ett studentkonto. Gå till länken: [http://www.github.com/edu](http://www.github.com/edu)
Välj **I'm a student** och **sign in here** och följ instruktionerna. Efter denna process bör du få ett e-postmeddelande från github och du har möjlighet att skapa privata så kallade repositorier. Oftast kommer du använda ett repositorie per kurs.


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
