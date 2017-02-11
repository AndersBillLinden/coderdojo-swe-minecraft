# Inledning

Detta är ett research-dokument för att utröna hur command blocks och redstone fungerar. Att läsa det här innan man skall ha coder dojo med command blocks/redstone-maskiner kan vara en bra idé för att förbereda sig på frågor från elever.

Informationen är framtagen genom att läsa minecrafts källkod samt genom att skriva mod i Java för att ta reda på vad olika variabler innehåller vid körning.

# Inledning
Command blocks kör kommandon med samma nivå som en admin. Det går inte att crafta dem eller hitta dem i creative-menyn. En admin måste använda

````
/give anders command_block
````

för att ge en spelare som heter anders ett command block. Man har bara glädje av ett command block om man är admin för att det går varken att bygga dem eller riva dem annars. Om en spelare som inte är admin stöter på ett command block händer inget om man högerklickar på det.

# Typer

Det finns 3 olika typer av command blocks: repeat, impulse, chain och repeat. Färgen på blocket avspeglas av typen.

Ett command block kan vara antingen always active eller needs redstone.

Det kan vara conditional eller unconditional.

# Needs redstone

Om ett block behöver redstone för att köras så måste någon av de fyra blocken vid sidorna eller blocket under ha redstone power.

# Redstone power

Redstone dust som är powered kraftsätter blocket under och blocken vid sidorna (om dessa inte är luft). En aktiv redstone torch däremot kraftsätter inte blocket under utan över.

Vilket solitt block som helst kan vara kraftsatt. Om en lampa är
bredvid ett kraftsatt block i vilken riktning som helst så lyser den. Den blir däremot inte kraftsatt (då skulle man kunna bygga ett kluster av lysande lampor).

# Redstone torch

En torch kan vara både input och output. Som output så ger den alltid en redstonesignal med styrkan 15. Som input så agerar den NOT, dvs är släckt om insignalen är hög, tänd om den är låg.

Det enda sättet att kraftsätta ett block med en redstone torch är att placera den under blocket såvida det inte är ett command block eller redstone wire. Redstone torches som man placerar bredvid varandra påverkar inte varandra. Inte heller om det är ovanför varandra (vilket de ju kan vara om man sätter dem på en vägg).

# Levers

Om en lever som är monterad vertikalt pekar uppåt är den avstängd, nedåt påslagen.

# Frågor och svar

F: Om man bygger ett command block som är repeterande, always active och skriver in kommandot `/say hej` så att det sätter igång och skickar chatmeddelanden och därefter sätter en komparator efter kommandblocket så kommer den att bli aktiverad. Om man  högerklickar på commandblocket och väljer needs redstone och trycker done så kommer komparatorn fortfarande vara aktiv (A). Om man högerklickar igen och bara klickar done så kommer komparatorn att bli inaktiverad. Varför då?

S: Om man bryter redstone-komparatorn efter (A) och sätter dit den igen så kommer den fortfarande att vara aktiverad. Man måste öppna menyn i command blocket och trycka done en extra gång för att en komparator efter commandblocket skall vara inaktiv.

