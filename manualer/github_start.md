Github - Hur du hanterar dina utvecklingsfiler
==============================================

Denna handledning innehåller en introduktion till git och github, varför vi vill att du använder github i undervisningen samt en guide hur du kommer igång att jobbar med git och github på mac och windows.
För att hänga med i guiden krävs grundläggande datorkunskap.

Vad är git och github?
--------

[git](http://git-scm.com/ "Den officella sidan om git") är ett versionhanteringssytem som är utarbetat främst för utvecklare och hantering av kod. Med versionshanteringssytem menas att systemet hjälper utvecklare att hantera alla de filer som oftast ingår i ett utvecklingsprojekt. Det ger möjligheter för flera utvecklare att kunna arbeta med samma filer utan att riskera att man skriver över någon annans arbete. Varje gång man ändrar i en fil sparas den som en ny version. Man kan också gå tillbaka i versionerna för att komma tillbaka till ett utgångsläge.

Ni kommer under er utbildning att använda er av git samt andra versionhanteringssytem så som t.ex. subversion (svn).
Git skapades av [Linus Torvalls](http://sv.wikipedia.org/wiki/Linus_Torvalds "Linus Torvalds wikipedia"), ett namn som säkert många känner till som skaparen till operativsystemet Linux. Git uppkom helt enkelt för att Linus inte tyckte att det fanns bra fritt versionhanteringssystem som kunde hantera all kod som Linux består av och alla de utvecklare som är inblandade i projektet. 

I många av våra kurser som vi använda tjänsten [github](http://github.com/ "Githubs hemsida") som använder sig av git. Github är en tjänst som ger oss som utvecklare möjlighet att, via webben, skapa, hantera och lagra projekt via git. Github ger oss också möjlighet att dela kod med andra, studera andras kod och använda andras kod för att bygga nya applikationer eller föreslå förändringar. Github är alltså en tjänst för "social coding". Man kan dock också använda github för att dela utvecklingsfiler i privata grupper eller som ensam utvecklare hantera sina filer.

Tre vanlig aord som används på github är:

* "forking" - Detta iinebär att man hittar ett intressant projekt som någon annan lagt ut. "Forkar" man då detta projekt får man en kompia av alla filer som man kan fortsätta jobba med efter eget huvud.
* "pull request" - Detta innebär att du har forkat ett projekt och gjort förändringar som du vill dela med dig av till orginalprojketet
* "merge" - Om ägaren av orginalprojketet tycker att dina ändringar är bra kan hon/han välja att baka in dessa i orginalkoden d.v.s. göra en "merge"

Här är några fler resurser kring git och github:
[Introduction to Git with Scott Chacon of GitHub](http://www.youtube.com/watch?v=ZDR433b0HJY "Youtubevideo om git")

Varför vill vi att du använder github?
---

I många av våra kurser kommer det vara krav på att använda github för att hantera sina kodfiler. Detta beror på flera saker:

* Först och främst kommer git och github vara något du med säkerhet kommer stöta på i ditt kommande arbetsliv och många arbetsgivare kan se det som en merit att ha erfarenhet av detta.
* Du kommer enklare kunna hantera dina filer. Inga datorkrasher kommer få dina filer att försvinna, du kan komma åt dina filer från flera olika datorer och enheter.
* Du kan enkelt dela dina filer med dina lärare. Vid examinering av t.ex. koduppgifter vill läraren titta på din kod och kan då via github enkelt dela dessa. Vid t.ex. frågor kring eller problem med din kod kan läraren enkelt komma åt den senaste versionen.
* I vissa kurser kommer ni att arbeta i grupper och github ger en bra möjlighet att sammarbeta kring kodfilerna.
* Github är ett kraftfullt verktyg för att studera och lära sig av andras kod.
* Läraren kan följa dina versioner och se hur du ligger till i kursen.


Hur börjar man med github?
---
Det första Du bör göra är att [skapa dig ett konto på github](http://www.github.com). Här är det viktigt att du __registrar dig med din studentmejl från LNU__. Detta för att du ska kunna registrera ett education-konto och på så sätt kunna ksap vad man kallar privata repositorier, alltså kodprojekt som ingen annan än du kan se. Välj också gärna ett användarnamn som innehåller ditt användarnamn här på LNU.

![Skapa ett konto på github][github_reg] 

Fyll i formuläret som ovan fast med ditt eget användarnamn.


[github_reg]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_register.png "Github registration"





	- Skapa konto, registrera dig med användarnamn
	- Uppdatera till education
	- Skapa ett nytt repositorie, dela det med lärare
	- Ladda ner och installera en klient (mac och windows)
	- Börja utveckla
		- Sync och commit
		- Ändra och commit
		- View history
		
	- github pages
