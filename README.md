# Command blocks

Ett command block kan man inte få på något annat sätt än att en admin kör kommandot

````
@give spelarnamn command_block
````

För att ge sig själv ett command block kan man använda

````
@give @p command_block
````



# Uppgifter

## Självöppnande dörr

En dörr som öppnar sig när spelaren kommer i närheten. Dörren får sin power från en redstone wire som är belägen diagonalt nedanför den. Maskinen kräver
förutom ett commandblock även en comparator och en repeater samt redstone dust (wire).

![screenshot](https://raw.githubusercontent.com/AndersBillLinden/coderdojo-swe-minecraft/master/screenshots/open_door_automatically.png?token=AA-Gepe5nP8Ipha4oeo__K9Co2idoB4aks5Yo3EWwA%3D%3D)

Commandblocket är repeating, always active och har kommandot:

````
/testfor @p[r=5]
````

## Gömd ingång

Mha kommandot /clone kan ett avsnitt av block kopieras till en annan koordinat och med /fill kan man fylla ett område med t.ex. luft (air). Detta kan man kombinera och göra en "gömd ingång".

![screenshot](https://raw.githubusercontent.com/AndersBillLinden/coderdojo-swe-minecraft/master/screenshots/secret_passage1.png?token=AA-GevKTx6yq8dh_AaDgaQPo9XqEh9zWks5YqMD7wA%3D%3D)

Detta är en gömd igång, när man kommer närmare så försvinner en del av strukturen

![screenshot](https://raw.githubusercontent.com/AndersBillLinden/coderdojo-swe-minecraft/master/screenshots/secret_passage2.png?token=AA-Gelp2hdGtgf_TUxKnn0gGgIIHFK7sks5YqMFnwA%3D%3D)

## Repeterande ljud

## Teleporter

## Ett får som byter färg med jämna mellanrum

## En vallgrav som byter från vatten till lava när man kommer i närheten



# Användbara kommandon

## Stänga av output från commandblocks

T.ex. stänga av output from kommandot /testfor som är  i stil med [@: Found spelare].

````
/gamerule commandBlockOutput false
````

## Byta ut alla block av en viss typ mot en annan

````
/fill ~-20 ~-8 ~-20 ~20 ~8 ~20 mycelium 0 replace grass
````

## Klippa gräset

````
/fill ~-20 ~-8 ~-20 ~20 ~8 ~20 air 0 replace tallgrass
````

## Spela ljud

När man skriver in namnet på ljudet så använder man med fördel TAB för att få komplettering. @a betyder att alla spelare kan höra ljudet.

````
/playsound minecraft:entity.ghast.death master @a ~ ~ ~
````

