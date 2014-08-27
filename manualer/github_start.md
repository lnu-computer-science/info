Denna handledning innehåller en kort introduktion till Git och Github samt en förklaring till varför vi vill att du använder dessa tjänster i våra kurser. Du kommer också i denna handledning få en introduktion till hur du börjar arbeta med Git. Observera dock att enskilda kurser kan ha olika krav på hur man ska använda Git och Github men det framgår i så fall av respektive kurs webbplats. Denna guide är inte en komplett handledning till Git utan kan ses som en startpunkt för att komma igång. Vi rekommenderar även den kostnadsfria boken [Pro Git](http://git-scm.com/book) som är fullmatad med nyttig information kring Git för djupare förståelse. 

För att hänga med i guiden utgår vi från att du har en grundläggande datorkunskap.

Har du tidigare arbetat med Git/Github kan du mycket väl ha invanda arbetssätt som du är fri att använda även i våra kurser, men läs igenom guiden nedan och eventuella krav respektive kurs har.

##Vad är Git och Github?

[Git](http://git-scm.com/ "Den officella sidan om git") är ett versionhanteringssytem som är utarbetat främst för mjukvaruutvecklare och hantering av kod, speciellt i större projekt med flera utvecklare som jobbar mot samma kod. Med ett [versionshanteringssystem](http://sv.wikipedia.org/wiki/Versionshantering) menas att systemet hjälper användarna att hantera filer och spara dem i olika versioner så att man kan spåra förändringar och t.ex. gå tillbaka i historiken. Det ger också möjligheter för flera utvecklare att dela och kunna samarbeta kring gemensamma filer utan att riskera att man skriver över någon annans arbete. Du kommer under din utbildning att använda dig mycket av Git men även stöta på andra versionhanteringssytem så som t.ex. Subversion (svn). [Mer information om versionshantering](http://git-scm.com/book/en/Getting-Started-About-Version-Control).

Git skapades av [Linus Torvalls](http://sv.wikipedia.org/wiki/Linus_Torvalds "Linus Torvalds wikipedia"), ett namn som säkert många känner till som skaparen till operativsystemet Linux. [Git uppkom](http://git-scm.com/book/en/Getting-Started-A-Short-History-of-Git) helt enkelt för att Linus inte tyckte att det fanns ett bra och fritt versionhanteringssystem som kunde hantera all kod som Linux består av och underlätta för alla de olika utvecklare som är inblandade i utvecklingen av operativsystemet. 

I många av våra kurser kommer vi också använda tjänsten [Github](http://github.com/ "Githubs hemsida"). Github är en tjänst som ger oss utvecklare möjlighet att, via webben, skapa, hantera och lagra projekt och dess data via Git. Github ger oss också möjlighet att dela kod med andra, studera andras kod och använda andras kod för att bygga vidare på. Github är alltså en tjänst för "social coding". Man kan också använda github för att dela utvecklingsfiler i privata grupper eller som ensam utvecklare hantera sina filer på ett smidigt sätt. Vi skulle kunna kalla det ett slags Facebook, fast för kod. På senare tid har dock allt fler upptäckt möjligheterna med Git och Github och nu för tiden hittar man inte bara mjukvaruprojekt på Github utan används även av författare, lärare och en mängd andra branscher. Ta t.ex. en titt på [Government Github](https://government.github.com/).


##Varför vill vi att du använder Git och Github?

I många av våra kurser kommer det vara krav på att använda Git och Github för att hantera kod och dokumentation. Detta beror på flera saker:

* Först och främst kommer Git och Github vara något du med säkerhet kommer stöta på i ditt kommande arbetsliv.
* Ditt Github-konto kommer fungera som ett CV där du samlar dina projekt och där eventuella arbetsgivare kan se vad du kan och har producerat tidigare. Detta är något vi märker fler och fler arbetsgivare tycker är viktigt så att redan från början bygga upp sitt Githubkonto bör vara en viktig punkt i din utveckling.
* Du kommer enklare kunna hantera dina filer. Inga datorkrasher kommer få dina filer att försvinna (om du är noga med att synka dina filer med Github). Du kan också komma åt dina filer från flera olika datorer och enheter.
* Du kan enkelt dela dina filer med dina lärare. Vid examinering av t.ex. koduppgifter vill läraren titta på din kod och kan då via Github enkelt komma åt denna. Vid t.ex. frågor kring eller problem med din kod kan läraren enkelt komma åt den senaste versionen.
* I vissa kurser kommer ni att arbeta i grupper och Github ger en bra möjlighet att sammarbeta i mjukvaruprojekt.
* Github är ett kraftfullt verktyg för att studera och lära sig av andras kod.
* Läraren kan följa dina versioner och se hur du ligger till i kursen.
* Github har också ett system för att skriva kommentarer, ToDo-listor m.m som underlättar vid arbetsgången.


##Att börja med Github

När man börjar jobba med Git och Github kommer man stöta på vissa begrepp som är viktiga att känna till. Vanliga ord som vi kommer använda är:

* **Repositorie/Repository** - Kallar ofta förkortat för "repo" och är oftast ett projekt. Vi kan likna ett repositorie med en mapp/katalog innehållandes filer och undermappar som kan versionshanteras. Du skapar oftast ett repositorie per kurs eller ett repositorie per applikation.
* **Commit** - Att "commit:a" sina ändringar talar om att man nu har uppdaterat sina filer och sparar dessa i en ny version, en commit.
* **Forking** - Detta innebär att man hittar ett intressant projekt som någon annan lagt ut och som man själv vill bygga vidare på. "Forkar" man då projektet får man en kopia av alla filer som man kan fortsätta jobba vidare med på egen hand och kanske i slutändan föreslå dessa förändringar för orginalskaparen.
* **Pull request** - Detta innebär att du har forkat ett projekt/repositorie och gjort förändringar i detta som du vill dela med dig av till orginalprojketet. Du kan då föreslå detta för repositorie-ägaren genom att göra en "pull request" som ägaren får godkänna.
* **Merge** - Om ägaren av repositoriet tycker att dina ändringar är bra kan hon/han välja att baka in dessa i orginalkoden d.v.s. göra en "merge", en sammanslagning.
* **Branch/Branching** - Du kommer att använda "branching" eller förgreningar i ditt repro för att undvika att ändra i projektets huvudgren. Detta är extra viktigt då man är flera personer som samarbetar i samma repro.

Vi kommer återkomma till vissa av dessa begrepp längre ner i texten.

###Skapa ditt studentkonto på Github
Det första Du bör göra är att [skapa dig ett konto på github](http://www.github.com). Här är det viktigt att du __registrar dig med din studentmejl från LNU__. Detta för att du ska kunna registrera ett education-konto och på så sätt kunna skapa vad man kallar privata repositorier, alltså kodprojekt som ingen annan än du och de du väljer att samarbeta med kan se. Välj ett användarnamn som är eller innehåller ditt användarnamn här på LNU.

![Skapa ett konto på github][github_reg] 

Fyll i formuläret som ovan fast med ditt eget användarnamn.


###Uppgradera ditt github-konto till education

Nästa steg är att registrera detta nyskapade konto som ett studentkonto. Gå till länken: [http://www.github.com/edu](http://www.github.com/edu)
Välj **Request a discount**, logga in om du inte gjort det och välj sedan **Student**, klicka på nästa och följ instruktionerna. Efter denna process bör du få ett e-postmeddelande från Github och du har möjlighet att skapa upp till fem privata repositorier. 


###Skapa ett repositorie
Nu är det dags att skapa ditt första repositorie. Det gör du från din startsida på github när du loggat in.

<img src="https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_startpage.png" width="80%" />

Klicka på knappen "New repository" och fyll i dina uppgifter. Går du en kurs har du säkert fått information om vad du ska döpa detta repositorie till. Var noga med detta!

![Githubs - skapa ett nytt repositorie][github_repo_new] 

Du kan här välja om du vill skapa ditt repositorie public (alla kan se din kod) eller private. Bara du och de du delar ditt repositorie med kan se dina filer. 

##Att börja använda Git
Vi ska nu börja titta på hur vi arbetar med Git. Denna guide har valt att koncentrera sig på hur man arbetar med Git via ett terminalfönster. Det finns grafiska klienter att använda men dessa får du själv upptäcka när du väl lärt dig grunderna i Git-kommandon. Du kommer arbeta med terminalfönster mycket under din utbildning så att bli van vid detta är viktigt.

## Installera Git på din dator
Om du arbetar på en egen dator är det en bra start att börja med att installera Git. Använder du skolans datorer bör det redan vara installerat på dessa. Att installera Git är inte svårare än att installera något annat program. Du laddar ner och installerar en körbar fil. [Mer information hittar du på Git:s officiella sida](http://git-scm.com/book/en/Getting-Started-Installing-Git). Välj sätt att installera på beroende på ditt operativsystem. Om du vill kan du välja de standardalternativ som följe rmed installationsguiden.

### Konfigurera Git
För att på ett enkelt sätt komma igång kan vi börja med att konfiguera Git genom att tala om vem vi är.

#### *Mac*
Öppna terminalfönstret genom att söka upp det i "Spotlight" (programmet heter Terminal) eller via Finder "Go" --> "Utilities" --> "Terminal". Vi detta terminalfönster kan du sedan börja skriva Git-kommandon.

#### *Windows*
Har du installerat Git från installationsfilen bör du i din startmeny fått ett alternativ "Git". Du öppnar ett terminalfönster för Git i Windows genom att du går via startmeny --> "Git" --> "Git bash".

![Git Bash][git_bash] 


### De första inställningarna
Börja med att testa att din installation är korrekt genom att skriva:

`git --version`

Du bör då få upp en bild liknande denna (skärmdumpen är tagin i windows - kan se annorlunda ut i t.ex. Mac):

![Git Version][git_version] 

Forsätt genom att ange dina uppgifter i konfigurationen för Git. Använd såklart ditt namn och e-postadress (din studentaddress)

`git config --global user.name "John Doe"`

`git config --global user.email johndoe@example.com`

Kontrollera dina inställningar via:

`git config --list`

![Git Config][git_config] 

## Att skapa ett repositorie
Ett centralt begrepp inom Git är repositorie (repository) eller ofta förkortat som "repo". Detta kan förklaras som ett versionshanterat projekt. Du skapar oftast ett repositorie per kurs eller per applikation. Ett repositorie kan skapa på olika sätt. Antingen via att skapa ett helt nytt repo på din lokala dator eller genom att ladda ner ett redan påbörjat repo från t.ex. Github.

### Skapa ett nytt lokalt repositorie
Börja med att använda kommandot cd i terminalen för att bege dig till någon lämplig katalog där du vill skapa ditt repositorie. Har du ingen erfarenhet av dessa typer av kommandon (UNIX-kommandon) kan vi rekommendera [Ubuntu-manualens korta introduktion till de vanligaste](http://help.ubuntu-se.org/10.04/basic-commands/sv/files-directories-commands.html). Väl i hemkatalogen skapar du en ny mapp genom att skriva:

`mkdir my-application`

Detta skapar en katalog med namnet my-application. För att skapa ett repositorie i denna mapp navigerar du dig in i mappen och där skriver

`git init`

Du har nu skapat ett helt eget lokalt repositorie och har förmodligen fått en mapp som heter ".git" (kan vara dold i filhanteraren). Den mappen innehåller all information om detta repositorie och de versionsförändringar vi kommer göra. Denna mapp ska du alltså inte bry dig om så mycket utan bara låta Git sköta om. Du kan nu testa statusen på ditt repo genom att skriva:

`git status`

Vi har ännu inte lagt till några filer i vår versionshanterade katalog (vårt repo). Så skapa en fil index.html och spara i katalogen du nyss skapade. Kontrollera nu statusen igen med `git status` och observera nu skillnaden.

Git har alltså upptäckt att vi lagt till en ny fil i mappen och talar om att denna inte är versionshanterad. Varje fil i en mapp som är Git-hanterad kan antingen vara "tracked" eller "untracked". För att lägga till filen index.html vi nyss skapade skriver du:

`git add index.html`

Ovanstående kommando lägger till just filen index.html. Har man skapat flera filer samtidigt som vill lägga till använder man:

`git add .`

Vilket också är det vanligaste fallet. Kolla nu status på ditt repositorie igen med `git status`.

Filen är nu tillagd i vad man kallar "staging area" men den är fortfarande inte helt versionshanterad. Vi måste också göra en så kallad "commit" för att få till detta. En "commit" gör man när man suttit och jobbat ett tag med något, kanske skrivit en deluppgift, implementerat en funktion i sin applikation eller kanske bara tar en paus och vill spara undan det man gjort hittils. Man brukar säga att man ska "commit:a" sin kod ofta men inte så att det blir absurt. En "commit" ska också innehålla en bra kommentar som beskriver för andra vad du gjort sedan sist. Även om du kommer jobba ensam i vissa repositorier så var noga med att skriva bra och förklarande kommentarer till dina commit:s. För att göra en commit skriver du i terminalfönstret:

`git commit -m "Jag har precis skapat filen index.html. Den är dock fortfarande tom"`

Du bör såklart byta ut kommentaren innanför citattecknen mot en kommentar som passar i ditt fall, Kontrollera nu ditt repositories status

`git status`

Testa nu att göra en ändring i filen index.html samt skapa en ny fil och lägg i mappen. Kolla status, lägg till den nya filen med 

`git add .` 

och gör en ny commit. Du bör nu ha ett lokalt repositorie med två versionshanterade filer och två stycken "commits".

### Skapa ett repositorie på Github och klona ner lokalt
Men om man har ett repositorie på Github och vill utveckla lokalt på sin dator och sedan skicka upp förändringarna. Hur gör man då?

Börja med att skapa ett repositorie på ditt konto på Github.
På ditt nya repositories första sida, nere till höger, kommer du se något som heter "HTTPS clone URL". Kopiera den sökväg som finns där. Den ska vi nu använda via terminalfönstret klona ner en kopia av repositoriet och få en koppling så vi kan skicka upp våra förändringar.

Gå till terminalfönstret och navigera dig till den mapp där du vill kopiera ner repositoriet och skriv:

`git clone https://github.com/xx222xx/myRepo.git`

där den sista delen är den address du kopierade. Du har nu sparat ner en exakt kopia av det som låg på github. Alla filerna bör ha hamnat i en mapp som om man tittar på addressen ovan borde heta "myRepo". Du har nu ett lokalt skapat repositorie och kan jobba vidare med "add" och "commit" under arbetets gång. Observera dock att dessa förändringar bara sker lokalt än så länge.

## Skicka upp förändringar till github
Vi har nu arbetat på ett tag men som sagt har vi bara gjort våra förändringar lokalt på den dator vi arbetar på för tillfället. Vi vill ju gärna spara dem centralt på Githubs server så vi kan komma åt dem från vilken dator som helst eller kanske är vi flera som jobbar i samma projekt. Kanske ör det så att du nu suttit i skolan och jobbat och vill nu gå hem och arbeta vidare på din dator hemma. Naturligtvis måste vi skicka upp förändringarna till Github så vi kan komma åt dem från en annan dator.
För att göra detta skriver du i terminalfönstret:

`git push`

Man kan nu kontrollera att förändringarna finns på Github och man kan nu klona ner dessa på liknande särr till en annan dator man vill jobba vidare på.


## Övning
Nu ska du få testa lite själv. Din uppgift blir nu följande.

1. Logga in på ditt Githubkonto och skapa ett nytt repositorie där. Skapa en readme-fil och en ignore-fil i repositoriet. [Läs mer om ignore-filer](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Ignoring-Files).
2. Skapa en katalog med namnet "projects", via terminalfönstret, på lämplig plats i ditt filsystem. 
3. Klona nu ut repositoriet till din lokala dator till den mapp du nyss skapade.
4. Skapa en ny fil, index.html, och lägg till den i repositoriet och skicka sedan upp till github. Besök sidan för ditt github-repositorie och kontrollera att filen finns där.
5. Gör en mindre förändring i index.html samt skapa en ny fil, contacts.html. Se nu till att den nya filen och den nya förändringen hamnar i en ny commit upp på github.
6. Skapa en ny mapp, "projects_simulate" för att simulera att vi nu satt oss och jobba vid en ny dator. Klona nu ner repositoriet på nytt till denna mapp och kontrollera att det har alla de uppdaterade filerna med sig.
7. Gör en förändring i någon av filerna och gör en commit på detta. Skicka sedan upp det till github igen. Kontrollera att förändringen kom med.
8. Gå nu tillbaka till den första mappen "projects". Kontrollera statusen. Du bör där se att den senaste förändringen som finns på github inte finns där ännu. Vi måste på något sätt ladda ner den innan vi kan fortsätta jobba. Annars kommer vi hamna i osynk och det vill vi inte. Det är därför viktigt att via terminalfönstret ställer oss i mappen och kör kommandot:
	*git pull*
	Det bör ladda ner de förändringar som gjorts och vi får samma version som finns på github. Vi kan nu fortsätta jobba med filerna.

Här hittar du två filmer där vi visar hur man kan lösa uppgiften ovan. 

[Film inspelad i Windows för punkt 1-5](http://orion.lnu.se/pub/information/coursepress/info/video/git/git_win.mp4)

[Film inspelad i Mac för punkt 6-8](http://orion.lnu.se/pub/information/coursepress/info/video/git/git_mac.mp4)

##Branching
Ytterligare ett begrepp vi måste känna till är Branch eller Branching. Det är en finess som är oumbärlig när man börja jobba flera personer inom samma projekt. Med en branch menar man att man skapar en förgrening i aktuellt projekt. Det är vanligt förekommande att man t.ex. skapar en ny branch när man ska införa en ny funktion i en applikation. Man skapar då en branch där man jobbar med koden till denna funktion utan att påverka själva huvudspåret. Man kan alltså säga att en branch är en tillfällig kopia som används under tiden en ny funktion implementeras för att sedan slås ihop (genom en så kallad "merge") med själva huvudspåret (som alltid kallas master). För att få en tydligare bild av vad branchning är rekommenderas [vidare läsning i git-boken](http://git-scm.com/book/en/Git-Branching-What-a-Branch-Is).

OK, säg då att vi vill jobba med en branch. Kanske är det en funktion eller webbsida som vi ska skapa i ett gemmensamt projekt som vi vill se till att vi har i en egen branch under tiden vi jobbar med den. För att sedan slå ihop med själva huvudspåret när vi anser oss klara med funktionen.

Vi ser till att vi i vårt terminalfönster befinner oss i vår versionshanterade mapp och kör kommandot

`git checkout -b my-new-branch`

Där my-new-branch är det namn du ger din branch. Kör nu `git status` så ser du att du nu befinner dig i din skapade branch. Alla add och commit kommer nu endast att påverka denna nya branch. Så under tiden du jobbar med funktionen gör du dina förändringar bara till denna förgrening av koden. När vi sedan känner oss klara med funktionen vi utvecklat vill vi såklart slå ihop våra förändringar med huvudspåret (som egentligen är en branch som kallas "master"). Detta gör vi genom en så kallad megre.
Detta gör man i två steg. Först måste vi förflytta oss tillbaka till vår master-branch och sedan tala om att vi vill göra en merge från vår egna branch. Kör följande kommandon:

`git checkout master
git merge my-new-branch`

Sen bör man naturligtvis köra en `git push` för att skicka upp våra förändringar. Detta brukar vara ett vanligt arbetsflöde när man jobbar med git. Vi kan rekommendera att skriva ut [följande bild](https://www.sonassi.com/wp-content/uploads/2012/07/simple_git_daily_workflow.pdf) för att ha som stöd när man jobbar med Git och Branches.

Detta ska förhoppningsvis gett lite information kring hur du kommer igång med Git och Github. Vi kan vidare rekommendera att du tittar upp följande länkar för ytterligare information:

* [Den interaktiva guiden som github har](https://try.github.io). Den tar upp fler saker än vad vi lärt oss hittils men det kan ändå vara ett bra läge att köra den nu

* Du bör också skaffa dig förståelse för [taggning](http://git-scm.com/book/en/Git-Basics-Tagging) och [hur man går tillbaka i historiken av sina commits](http://git-scm.com/book/en/Git-Basics-Undoing-Things).

* [Ett så kallat Cheat Sheet](http://www.git-tower.com/blog/git-cheat-sheet/) som tar upp de vanligaste Git-kommandona samt även [en enklare referens](http://gitref.org/) till dessa kommandon


Föreslå förändringar på denna handledning
------------------------------------------
Detta dokument ligger på [github](https://github.com/LNU-CoursePress/info/blob/master/manualer/github_start.md) och hittar du felaktigheter eller vill föreslå förändringar går det bra att göra det där.


[github_reg]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_register.png "Github registration"
[github_reg_edu]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_register_edu.png "Github registration education"
[github_startpage]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_startpage.png "Github startpage"
[github_repo_new]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_repo_new.png "New repository"
[github_settings]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_settings.png "Settings"
[github_collaborator]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/github_collaborator.png "github_collaborator"
[git_bash]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/git_bash.png "git_bash"
[git_version]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/git_version.png "git_version"
[git_config]: https://raw.github.com/LNU-CoursePress/info/master/manualer/images/git_config.png "git_config"
