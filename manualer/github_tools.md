## Github - Där dina filer sparas

I denna kursen ska vi använda ett versionshanteringssytem för hantering av de filer du skapar. Systemet heter Git och är väl använt, främst inom programvarutveckling. En väldigt populär tjänst där utvecklare samlar sin kod är [github.com](//github.com). Det är den tjänsten som vi ska använda i denna kurs och det är där du alltså ska spara din kod och också där vi kursansvariga kommer åt din kod. Vi vill alltså *inte* ha några mejl med kod inskickad.

[Läs på om git och github i denna guide.](//coursepress.lnu.se/info/manual/kom-igang-med-github/). Se till att skapa ett konto på github enligt de instruktioner som finns där.  


## Utvecklingsverktyg (IDE)
Du är fri att själv välja vilken utvecklingsmiljö (IDE, integrerad utvecklingsmiljö) du ska använda i denna kurs. Dock behöver du säkert lite mer information för att kunna ta ställning till denna. Här kommer tre olika alternativ man kan välja.

## 1. Cloud9 med integrerad koppling till github - Passar både campus- och distansstudenter
Cloud9 är en helt webbaserad utvecklingsmiljö. Det är en enkel lösning som smidigt kopplas ihop med github. Du slipper göra några installationer utan kan använda din webbläsare och skriva din kod direkt i den. Dock ska vi redan nu säga att cloud9, som är en gratistjänst, har den dåliga vanan att det upplevs väldigt segt (speciellt på eftermiddagar och kvällar) och ibland får man starta om webbläsaren för att kunna fortsätta arbeta. Man kan alltid börja utveckla i denna miljö men märker man att strular för mycket kan man enkelt byta sätt. Alla dina filer ska vi försöka spara centralt på github och dessa kan du alltid komma åt oavsett vilken IDE/editor du använder.

Cloud9 är en molnbaserad utvecklingsmiljö med stark integrering mot GitHub. Detta betyder att du kan låta Cloud9 klona ditt repositorie från GitHub utan att du behöver hämta hem dessa filer till din lokala dator, utan använder bara din webbläsare. Detta ger en stor fördel i att du enkelt kan påbörja arbete på en dator och avsluta på en annan utan att behöva flytta någon fil.

Här nedan följer en guide för hur du kommer igång med cloud9 och github och börjar utveckla:

1. Logga in på GitHub med ditt sedan tidigare skapade konto. 

2. Gå till [https://c9.io/](https://c9.io/) och välj att logga in via GitHub.<br />
	![Logga in på Cloud9 via GitHub][c9-login]

3. Acceptera att Cloud9 får komma åt ditt GitHub-konto.

4. Du kommer att klara dig bra på gratisvarianten av Cloud9 för kursernas skull så klicka bort rutan om att uppgradera till en betalningsplan.

5. Du bör nu se ditt/dina GitHub-repositorie i vänstermenyn. Klicka på den du vill använda.

6. För att klona repositoriet till Cloud9 så att du kan börja editera dina filer så klickar du på "Clone to edit". Du får välja om du vill ha ditt projekt öppet eller privat. Vilket som går bra men om du vill att dina filer ska vara publikt åtkomliga för exempelvis valideringstjänster bör du välja "public".

7. Allt klart. Börja editera genom att klicka på "Start editing" och du bör få upp din kodeditor. Du är nu redo att köra igång och koda! För att testa och se resultatet av ditt kodande så kan du klicka på "Preview" i Cloud9. Då ser du förändringar så fort du sparar ett dokument.


### Cloud9 och GitHub
Cloud9 har inget stöd för Git i det grafiska gränssnittet utan du måste arbeta med kommandoprompten, terminalen, när du gör commits och trycker dina ändringar till GitHub. 

Terminalen bör du se i en flik längst ner i Cloud9:
<br />
![terminal](https://raw.github.com/1dv435/Kursmaterial/master/Laborationer/pics/c9-terminal.png)

### Uppgift att göra
Öppna nu filen "README.md" och gör någon förändring i denna och spara dina ändringar.
Vi ska nu göra en "commit" samt synka våra ändringar till GitHub. 

1. Skriv: `git add .` i terminalen och tryck enter. *Eventuellt nytillagda filer läggs nu till till versionshanteringen. Även några filer från Cloud9s konfiguration läggs till men vi bryr oss inte om det i nuläget.*

2. Gör en commit genom att exekvera (*skriva och trycka enter*) kommandot: `git commit -am 'Min första commit!'`

3. Synkronisera med GitHub-repositoriet genom att exekvera kommandot: `git push`

Nu kan du gå till din GitHub-sida och kontrollera att alla ändringar du gjort i din readme-fil också finns på GitHub. 
Steg 1 till 3 ska du upprepa efter varje isolerat problem du löst. Det gör att du får spårbarhet i din kod och enkelt kan gå tillbaka till tidigare versioner av din kod. *(`git add .`behöver du bara göra när du lägger till filer och `git push` gör du när du vill trycka upp alla ändringar till github.)

Du är nu redo att köra igång och koda! För att testa och se resultatet av ditt kodande så kan du klicka på "Preview" i Cloud9. Då ser du förändringar så fort du sparar ett dokument.

## 2. Eget val av editor och githubklienten - Passar bra för distansstudenter eller de som har egen dator
Vill man inte använda cloud9:s webbaserade möjlighet kan man installera en egen kodeditor och ändå kunna spara sin kod på github. Det finns mängder av olika kodeditorer att välja på. Ska jag rekommendera en populär är det:
[sublimetext.com](sublimetext.com). Det är en enkel men ändå kraftfull editor som kommer funka finemang i denna kurs.
Det finns såklart [andra alternativ](http://alternativeto.net/software/sublime-text) ifall man vill.

Dessa editorer gör att man jobbar med filerna lokalt på din egen dator och vi måste på något sätt ha ett program som skickar upp filerna till github-tjänsten. Vi kan då använda github:s egna programvara för detta.
Informationsfilmer hur man installerar och använder dessa hittar Du på:
[http://coursepress.lnu.se/info](http://coursepress.lnu.se/info/manual/githubklienter-macwin/)

#### Uppgift att göra
Försök nu göra samma uppgift som under rubriken "Cloud9 och GitHub" och ändra i filen README.md via din valda editor och skicka upp ändringen till github via githubklienten.

## 3. Dreamweaver och tortoisegit - Passar campusstudenter
I campussalarna (Ny104-Ny113, Ny227) finns [Tortoisegit](https://code.google.com/p/tortoisegit/) installerat för att kunna jobba på liknande sätt som med den officiella githubklienten (2). Tortoisegit använder du alltså för att synkronisera dina filer mellan den dator du sitter på och github.

Vi rekommenderar att du sparar ditt repositorie på p: eftersom du detta då inte raderas när du loggar ut. 

Detta är arbetsgången.

1. Börja med att bege dig till din githubsida och leta efter "HTTPS clone URL" (nere i högra hörnet). Kopiera den adress som står i textrutan där. Den bör se ut liknande: https://github.com/xx222xx/xx222xx-xyyxxx-laborationer.git
Denna adress ska vi använda när vi ska hämta ner ditt githubrepositorie till p:/. 
	
2. Skapa en mapp med lämpligt namn på p: och högerklicka i den mappen. Du bör då få upp olika alternativ varav ett säger "Git clone". I textrutan för URL, skriver du in adressen du kopierade från github. Tryck OK för att spara ner dina filer från github (det är möjligt att om du har ett privat repositorie får du ange användarnamn och lösenord). Du har nu synkat ner ditt github-repositorie till p:/.
<br />
![Clone window][clone]

3. Nu kan du börja att skapa nya filer och göra "commits" till github. Börja med att ändra i filen README.md (som nu bör ligga i din mapp).

4. Du vill nu skicka upp din ändring till github och ska därför göra en commit.  Högerklicka igen på mappen och välj "git Commit...". 

5. Du får nu upp ett fönster där dina ändrade filer finns (se till att de är ibockade och valda). Skriv ett commit-meddelande i rutan och tryck OK och tryck i nästa dialogruta på "Push".
	<br />
	![git commit][git_commit]
	<br />
	Här kan du få behöva ange ditt användarnamn och lösenord till github. 

6. I nästa dialogruta väljer du OK. Går allt vägen skickas nu dina filer upp tillsammans med ditt meddelande och du bör se förändringarna på din github-sida.
<br />
![git push][git_push]

6. Har du t.ex. suttit hemma och jobbat och skickat upp filer därifrån till github måste du innan du startar med ditt arbete i skolan högerklicka på mappen och välja "git sync" för att få ner förändringarna från github till p: och börja jobba därifrån.

## Slutligen
Var noga att skicka upp dina filer och ändringar varje gång du  gjort färdig en uppgift eller tar en paus o.s.v. På detta sätt har du alltid dina filer versionshanterade och slipper att tappa bort dem.


[clone]: https://raw.github.com/1dv435/Kursmaterial/master/Laborationer/pics/clone_tort.PNG

[git_commit]: https://raw.github.com/1dv435/Kursmaterial/master/Laborationer/pics/git_commit_tort.PNG

[git_push]: https://raw.github.com/1dv435/Kursmaterial/master/Laborationer/pics/git_push_tort.PNG

[github-add-repro]: https://github.com/1dv435/Kursmaterial/raw/master/Laborationer/pics/github-add-repro.png

[github-add-user]: https://github.com/1dv435/Kursmaterial/raw/master/Laborationer/pics/github-add-user.png

[github-add-ghpages]: https://github.com/1dv435/Kursmaterial/raw/master/Laborationer/pics/github-add-ghpages.png

[github-default-branch]: https://github.com/1dv435/Kursmaterial/raw/master/Laborationer/pics/github-default-branch.png

[github-release]: https://github.com/1dv435/Kursmaterial/raw/master/Laborationer/pics/github-release.png

[github-deletemaster]: https://github.com/1dv435/Kursmaterial/raw/master/Laborationer/pics/github-deletemaster.png

[c9-login]: https://raw.github.com/1dv435/Kursmaterial/master/Laborationer/pics/c9-login.png
