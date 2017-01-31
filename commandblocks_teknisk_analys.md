# Command blocks och redstone-kretsar
Detta �r ett research-dokument f�r att utr�na hur command blocks och redstone fungerar. Att l�sa det h�r innan man skall ha coder dojo med command blocks kan vara en bra id� f�r att f�rbereda sig p� fr�gor.

Informationen �r framtagen genom att l�sa minecrafts k�llkod samt genom att skriva mod i Java f�r att ta reda p� vad olika variabler inneh�ller vid k�rning.

# Inledning
Command blocks k�r kommandon med samma niv� som en admin. Det g�r inte att crafta dem eller hitta dem i creative-menyn. En admin m�ste anv�nda

````
/give anders command_block
````

f�r att ge en spelare som heter anders ett command block. Om man f�r ett command block kan man g�ra ett

# Typer

Det finns 3 olika typer av command blocks: repeat, impulse, chain och repeat. F�rgen p� blocket avspeglas av typen.

Ett command block kan vara antingen always active eller needs redstone.

Det kan vara conditional eller unconditional.

# Needs redstone

Om ett block beh�ver redstone f�r att k�ras s� m�ste n�gon av de fyra blocken vid sidorna eller blocket under ha redstone power.

# Redstone power

Redstone dust som �r powered krafts�tter blocket under och blocken vid sidorna (om dessa inte �r luft). En aktiv redstone torch d�remot krafts�tter inte blocket under utan �ver.

Vilket solitt block som helst kan vara kraftsatt. Om en lampa �r
bredvid ett kraftsatt block i vilken riktning som helst s� lyser den. Den blir d�remot inte kraftsatt (d� skulle man kunna bygga ett kluster av lysande lampor).

# Redstone torch

En torch kan vara b�de input och output. Som output s� ger den alltid en redstonesignal med styrkan 15. Som input s� agerar den NOT, dvs �r sl�ckt om insignalen �r h�g, t�nd om den �r l�g.

Det enda s�ttet att krafts�tta ett block med en redstone torch �r att placera den under blocket s�vida det inte �r ett command block eller redstone wire. Redstone torches som man placerar bredvid varandra p�verkar inte varandra. Inte heller om det �r ovanf�r varandra (vilket de ju kan vara om man s�tter dem p� en v�gg).



# Levers

Om en lever som �r monterad vertikalt pekar upp�t �r den avst�ngd, ned�t p�slagen.

