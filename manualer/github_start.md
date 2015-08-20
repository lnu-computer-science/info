Denna handledning innehåller en kort introduktion till Git och GitHub samt en förklaring till varför vi vill att du använder dessa tjänster i våra kurser. Du kommer också i denna handledning få en introduktion till hur du börjar arbeta med Git. Observera dock att enskilda kurser kan ha olika krav på hur man ska använda Git och GitHub men det framgår i så fall av respektive kurs webbplats. Denna guide är inte en komplett handledning till Git utan kan ses som en startpunkt för att komma igång. Vi rekommenderar även den kostnadsfria boken [Pro Git](http://git-scm.com/book) som är fullmatad med nyttig information kring Git för djupare förståelse. 

För att hänga med i guiden utgår vi från att du har en grundläggande datorkunskap.


##Vad är Git och GitHub?

[Git](http://git-scm.com/ "Den officella sidan om git") är ett versionhanteringssytem som är utarbetat främst för mjukvaruutvecklare och hantering av kod, speciellt i större projekt med flera utvecklare som jobbar mot samma kodbas. Med ett [versionshanteringssystem](http://sv.wikipedia.org/wiki/Versionshantering) menas att systemet hjälper användarna att hantera filer och spara dem i olika versioner så att man kan spåra förändringar och t.ex. gå tillbaka i historiken. Det ger också möjligheter för flera utvecklare att dela och kunna samarbeta kring gemensamma filer utan att riskera att man skriver över någon annans arbete. Du kommer under din utbildning att använda dig mycket av Git men även stöta på andra versionhanteringssytem så som t.ex. Subversion (svn). [Mer information om versionshantering](http://git-scm.com/book/en/Getting-Started-About-Version-Control).

Git skapades av [Linus Torvalds](http://sv.wikipedia.org/wiki/Linus_Torvalds "Linus Torvalds wikipedia"), ett namn som säkert många känner som skaparen till operativsystemet Linux. [Git uppkom](http://git-scm.com/book/en/Getting-Started-A-Short-History-of-Git) helt enkelt för att Linus inte tyckte att det fanns ett bra och fritt versionhanteringssystem som kunde hantera all kod som Linux består av och underlätta för alla de olika utvecklare som är inblandade i utvecklingen av operativsystemet. 

I många av våra kurser kommer vi också använda tjänsten [GitHub](http://github.com/ "GitHubs hemsida"). GitHub är en tjänst som ger oss utvecklare möjlighet att, via webben, skapa, hantera och lagra projekt och dess data via Git. GitHub ger oss också möjlighet att dela kod med andra, studera andras kod och använda andras kod för att bygga vidare på. GitHub är alltså en tjänst för "social coding". Man kan också använda GitHub för att dela utvecklingsfiler i privata grupper eller som ensam utvecklare hantera sina filer på ett smidigt sätt. Vi skulle kunna kalla det ett slags Facebook, fast för kod. På senare tid har dock allt fler upptäckt möjligheterna med Git och GitHub och nu för tiden hittar man inte bara mjukvaruprojekt på GitHub utan även författare, lärare och en mängd andra branscher. Ta t.ex. en titt på [Government GitHub](https://government.github.com/).


##Varför vill vi att du använder Git och GitHub?

I många av våra kurser kommer det vara krav på att använda Git och GitHub för att hantera kod och dokumentation. Detta beror på flera saker:

* Först och främst kommer Git och GitHub vara något du med säkerhet kommer stöta på i ditt kommande arbetsliv.
* Ditt GitHub-konto kommer fungera som ett CV där du samlar dina projekt och där eventuella arbetsgivare kan se vad du kan och har producerat tidigare. Detta är något vi märker fler och fler arbetsgivare tycker är viktigt så att redan från början bygga upp sitt GitHubkonto bör vara en viktig punkt i din utveckling.
* Du kommer enklare kunna hantera dina filer. Inga datorkrasher kommer få dina filer att försvinna (om du är noga med att synka dina filer med GitHub). Du kan också komma åt dina filer från flera olika datorer och enheter.
* Du kan enkelt dela dina filer med dina lärare. Vid examinering av t.ex. koduppgifter vill läraren titta på din kod och kan då via GitHub enkelt komma åt denna. Vid t.ex. frågor kring eller problem med din kod kan läraren enkelt komma åt den senaste versionen.
* I vissa kurser kommer ni att arbeta i grupper och GitHub ger en bra möjlighet att sammarbeta i mjukvaruprojekt.
* GitHub är ett kraftfullt verktyg för att studera och lära sig av andras kod.
* Läraren kan följa dina versioner och se hur du ligger till i kursen.
* GitHub har också ett system för att skriva kommentarer, ToDo-listor m.m som underlättar vid arbetsgången.


##Terminologi

När man börjar jobba med Git och GitHub kommer man stöta på vissa begrepp som är viktiga att känna till. Vanliga ord som vi kommer använda är:

* **Repositorie/Repository** - Kallas ofta förkortat för "repo" och är oftast ett projekt. Vi kan likna ett repositorie med en mapp/katalog innehållandes filer och undermappar som kan versionshanteras. Du skapar oftast ett repositorie per kurs eller ett repositorie per applikation.
* **Commit** - Att "commit:a" sina ändringar talar om att man nu har uppdaterat sina filer och sparar dessa i en ny version, en commit. Detta görs i lokalt på din dator.
* **Push** - Att "push:a" innebär att man tar de "commit:ade" filerna och skickar/pushar upp på en central server. I Vårt fall kommer detta oftast vara GitHubs server.
* **Forking** - Detta innebär att man hittar ett intressant projekt som någon annan lagt ut på GitHub och som man själv vill bygga vidare på. "Forkar" man då projektet får man en kopia av alla filer som man kan fortsätta jobba vidare med på egen hand och kanske i slutändan föreslå dessa förändringar för orginalskaparen.
* **Pull request** - Detta innebär att du har forkat ett projekt/repositorie och gjort förändringar i detta som du vill dela med dig av till orginalprojketet. Du kan då föreslå detta för repositorie-ägaren genom att göra en "pull request" som ägaren får godkänna.
* **Merge** - Om ägaren av repositoriet tycker att dina ändringar är bra kan hon/han välja att baka in dessa i orginalkoden d.v.s. göra en "merge", en sammanslagning.
* **Branch/Branching** - Du kommer att använda "branching" eller förgreningar i ditt repro för att undvika att ändra i projektets huvudgren. Detta är extra viktigt då man är flera personer som samarbetar i samma repro då man enklare kan jobba utan att skriva över varandras filer.


##Kom igång med GitHub
Det första Du bör göra är att [skapa dig ett konto på GitHub](http://www.GitHub.com). Här är det viktigt att du __registrar dig med din studentmejl från LNU__. Detta för att du ska kunna registrera ett education-konto och på så sätt kunna skapa vad man kallar privata repositorier, alltså kodprojekt som ingen annan än du och de du väljer att samarbeta med kan se. Välj ett användarnamn som är eller innehåller ditt användarnamn här på LNU.

![Skapa ett konto på GitHub][GitHub_reg] 

Fyll i formuläret som ovan fast med ditt eget användarnamn.


###Uppgradera ditt GitHub-konto till education

Nästa steg är att registrera detta nyskapade konto som ett studentkonto. Gå till länken: [http://www.github.com/edu](http://www.GitHub.com/edu)
Välj **Request a discount**, logga in om du inte gjort det och välj sedan **Student**, klicka på nästa och följ instruktionerna. Efter denna process bör du få ett e-postmeddelande från GitHub och du har möjlighet att skapa upp till fem privata repositorier. 

Lägg lite tid på att surfa runt på GitHub och testa gärna att skapa ett nytt eget repo.


###Skapa ett repositorie
Nu är det dags att skapa ditt första repositorie. Det gör du från din startsida på GitHub när du loggat in.

<img src="https://raw.GitHub.com/LNU-CoursePress/info/master/manualer/images/github_startpage.png" width="80%" />

Klicka på knappen "New repository" och fyll i dina uppgifter. Går du en kurs har du säkert fått information om vad du ska döpa detta repositorie till. Var noga med detta!

![GitHubs - skapa ett nytt repositorie][GitHub_repo_new] 

Du kan här välja om du vill skapa ditt repositorie public (alla kan se din kod) eller private. Bara du och de du delar ditt repositorie med kan se dina filer. 


[GitHub_reg]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_register.png "GitHub registration"
[GitHub_reg_edu]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_register_edu.png "GitHub registration education"
[GitHub_startpage]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_startpage.png "GitHub startpage"
[GitHub_repo_new]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_repo_new.png "New repository"
[GitHub_settings]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_settings.png "Settings"
[GitHub_collaborator]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_collaborator.png "GitHub_collaborator"
