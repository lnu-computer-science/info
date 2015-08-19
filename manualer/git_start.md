##Git
Git är ett versionssystem medans GitHub är en tjänst som använder sig av git för att bygga en webbplats.

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
Ett centralt begrepp inom Git är repositorie (repository) eller ofta förkortat som "repo". Detta kan förklaras som ett versionshanterat projekt. Du skapar oftast ett repositorie per kurs eller per applikation. Ett repositorie kan skapa på olika sätt. Antingen via att skapa ett helt nytt repo på din lokala dator eller genom att ladda ner ett redan påbörjat repo från t.ex. GitHub.

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

`git commit -m "I have created the file index.html, but it is still empty"`

Du bör såklart byta ut kommentaren innanför citattecknen mot en kommentar som passar i ditt fall. Det kan vara bra att skriva kommentarerna på engelska då man ibland stöter på problem med svenska tecken. Kontrollera nu ditt repositories status

`git status`

Testa nu att göra en ändring i filen index.html samt skapa en ny fil och lägg i mappen. Kolla status, lägg till den nya filen med 

`git add .` 

och gör en ny commit. Du bör nu ha ett lokalt repositorie med två versionshanterade filer och två stycken "commits".

### Skapa ett repositorie på GitHub och klona ner lokalt
Men om man har ett repositorie på GitHub och vill utveckla lokalt på sin dator och sedan skicka upp förändringarna. Hur gör man då?

Börja med att skapa ett repositorie på ditt konto på GitHub.
På ditt nya repositories första sida, nere till höger, kommer du se något som heter "HTTPS clone URL". Kopiera den sökväg som finns där. Den ska vi nu använda via terminalfönstret klona ner en kopia av repositoriet och få en koppling så vi kan skicka upp våra förändringar.

Gå till terminalfönstret och navigera dig till den mapp där du vill kopiera ner repositoriet och skriv:

`git clone https://github.com/xx222xx/myRepo.git`

där den sista delen är den address du kopierade. Du har nu sparat ner en exakt kopia av det som låg på GitHub. Alla filerna bör ha hamnat i en mapp som om man tittar på addressen ovan borde heta "myRepo". Du har nu ett lokalt skapat repositorie och kan jobba vidare med "add" och "commit" under arbetets gång. Observera dock att dessa förändringar bara sker lokalt än så länge.

## Skicka upp förändringar till GitHub
Vi har nu arbetat på ett tag men som sagt har vi bara gjort våra förändringar lokalt på den dator vi arbetar på för tillfället. Vi vill ju gärna spara dem centralt på GitHubs server så vi kan komma åt dem från vilken dator som helst eller kanske är vi flera som jobbar i samma projekt. Kanske ör det så att du nu suttit i skolan och jobbat och vill nu gå hem och arbeta vidare på din dator hemma. Naturligtvis måste vi skicka upp förändringarna till GitHub så vi kan komma åt dem från en annan dator.
För att göra detta skriver du i terminalfönstret:

`git push`

Man kan nu kontrollera att förändringarna finns på GitHub och man kan nu klona ner dessa på liknande särr till en annan dator man vill jobba vidare på.


## Övning
Nu ska du få testa lite själv. Din uppgift blir nu följande.

1. Logga in på ditt GitHubkonto och skapa ett nytt repositorie där. Skapa en readme-fil och en ignore-fil i repositoriet. [Läs mer om ignore-filer](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository#Ignoring-Files).
2. Skapa en katalog med namnet "projects", via terminalfönstret, på lämplig plats i ditt filsystem. 
3. Klona nu ut repositoriet till din lokala dator till den mapp du nyss skapade.
4. Skapa en ny fil, index.html, och lägg till den i repositoriet och skicka sedan upp till GitHub. Besök sidan för ditt GitHub-repositorie och kontrollera att filen finns där.
5. Gör en mindre förändring i index.html samt skapa en ny fil, contacts.html. Se nu till att den nya filen och den nya förändringen hamnar i en ny commit upp på GitHub.
6. Skapa en ny mapp, "projects_simulate" för att simulera att vi nu satt oss och jobba vid en ny dator. Klona nu ner repositoriet på nytt till denna mapp och kontrollera att det har alla de uppdaterade filerna med sig.
7. Gör en förändring i någon av filerna och gör en commit på detta. Skicka sedan upp det till GitHub igen. Kontrollera att förändringen kom med.
8. Gå nu tillbaka till den första mappen "projects". Kontrollera statusen. Du bör där se att den senaste förändringen som finns på GitHub inte finns där ännu. Vi måste på något sätt ladda ner den innan vi kan fortsätta jobba. Annars kommer vi hamna i osynk och det vill vi inte. Det är därför viktigt att via terminalfönstret ställer oss i mappen och kör kommandot:
	*git pull*
	Det bör ladda ner de förändringar som gjorts och vi får samma version som finns på GitHub. Vi kan nu fortsätta jobba med filerna.

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

Detta ska förhoppningsvis gett lite information kring hur du kommer igång med Git och GitHub. Vi kan vidare rekommendera att du tittar upp följande länkar för ytterligare information:

* [Den interaktiva guiden som GitHub har](https://try.GitHub.io). Den tar upp fler saker än vad vi lärt oss hittils men det kan ändå vara ett bra läge att köra den nu

* Du bör också skaffa dig förståelse för [taggning](http://git-scm.com/book/en/Git-Basics-Tagging) och [hur man går tillbaka i historiken av sina commits](http://git-scm.com/book/en/Git-Basics-Undoing-Things).

* [Ett så kallat Cheat Sheet](http://www.git-tower.com/blog/git-cheat-sheet/) som tar upp de vanligaste Git-kommandona samt även [en enklare referens](http://gitref.org/) till dessa kommandon


Föreslå förändringar på denna handledning
------------------------------------------
Detta dokument ligger på [GitHub](https://GitHub.com/LNU-CoursePress/info/blob/master/manualer/GitHub_start.md) och hittar du felaktigheter eller vill föreslå förändringar går det bra att göra det där.

