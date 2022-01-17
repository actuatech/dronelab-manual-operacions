# DIRECTRIUS DE BATERIES

La majoria dels fabricants de RPA utilitzen bateries de polímer de liti, conegudes com a bateries LiPo. Les bateries LiPo són generalment més potents, més lleugeres, més petites i tenen més capacitat que les de NiCd o NiMH, a més de no sofrir d'efecte memòria. Tanmateix, si es carreguen, s'emmagatzemen o es manipulen de manera inadequada poden arribar a ser extremadament perilloses.

> DJI ha desenvolupat bateries de vol intel·ligents per als seus RPA basades en el format de bateria LiPo. Tot i les funcions intel·ligents, és necessari seguir una sèrie de consells per assegurar-ne la seguretat i maximitzar la seva vida útil.

## Contingut

1. **[Conceptes bàsics](#conceptes-bàsics)**
2. **[Seguretat de bateries](#seguretat-de-bateries)**
3. **[Càrrega de bateries](#càrrega-de-bateries)**
4. **[Emmagatzematge de bateries](#emmagatzematge-de-bateries)**
5. **[Viatjar amb bateries](#viatjar-amb-bateries)**
6. **[Emparellament de bateries](#emparellament-de-bateries)**
7. **[Rebuig de bateries](#rebuig-de-bateries)**
8. **[App DJI Go 4](#app-dji-go-4)**
9. **[Annexos](#annexos)**

## Conceptes bàsics

Totes les bateries es defineixen segons un sistema de valors. Aprendre a llegir aquest sistema de valors és fonamental per a entendre i comparar les propietats d'una bateria i determinar quina configuració és necessària per a cada aplicació.

### Voltatge / Núm. de cel·les (S)

Les bateries LiPo estan formades per cel·les individuals connectades en sèrie, sens el voltatge total de la bateria la suma dels voltatges de cada cel·la. Cada cel·la en una bateria té un voltatge nominal de 3.7V. El voltatge nominal és un estàndard de la indústria, però no és el voltatge de la bateria completament carregada (normalment ~4.2V), ni de la bateria al 50% de càrrega (normalment ~3.85V), ni el voltatge de la bateria al 80% de descàrrega en repòs (normalment ~3.75%). Normalment es defineix el voltatge en funció del nombre de cel·les de la bateria (conegut com a *S*).

```
1S = 1 cel·la = 3.7V
2S = 2 cel·les = 7.4V
...
6S = 6 cel·les = 22.2V
```

El voltatge afecta directament les RPM dels motors *brushless*, sent possible augmentar la velocitat del RPA si els motors i l'ESC suporten majors voltatges, però una bateria amb més cel·les de la mateixa capacitat és més pesada i afecta el rendiment del RPA.

**Una bateria LiPo està dissenyada per treballar dins un rang de voltatge segur, de 3V a 4.2V. La descàrrega per sota 3V pot causar pèrdua de rendiment i danys irreversibles a la bateria. La sobrecàrrega per sobre de 4.2V és perillosa i pot eventualment causar un incendi.**

### Capacitat

La capacitat indica quant corrent pot emmagatzemar la bateria, i es mesura en mAh. Aquesta unitat indica la quantitat de corrent que es pot drenar de la bateria durant una hora fins que queda descarregada; com més corrent dreni el carregament, menys temps durarà la bateria.

Augmentar la capacitat perllonga el temps de vol, però també incrementa el pes i mida de la bateria. Existeix un equilibri entre la capacitat i el pes que afecta el temps de vol i l'agilitat del RPA.

Una major capacitat també atorga un major corrent de descàrrega.

### Taxa de descàrrega

La taxa de descàrrega (C-Rate) indica la velocitat a la qual es pot descarregar una bateria de manera segura, en funció de la capacitat de la bateria.

'Corrent màxim de descàrrega = Taxa de descàrrega * Capacitat'

Moltes bateries mostren la velocitat de descàrrega en contínua i també la velocitat de descàrrega en *burst mode*, que és una descàrrega de màxima potència durant molt poc temps (~10s).

### Taxa de càrrega

La taxa de càrrega és el corrent de càrrega més alt indicat pel fabricant al qual es pot carregar una bateria de manera segura.

'Corrent màxim de càrrega = Taxa de càrrega * Capacitat'

Aquest valor és un màxim segur, no un màxim òptim. Carregar les bateries amb un corrent màxim de càrrega disminueix la vida útil de les bateries.

## Seguretat de bateries

Utilitzar sempre bateries oficials o aprovades pel fabricant. Llegir el manual de la bateria i entendre la seva funcionalitat bàsica. No comprar mai bateries de segona mà.

No utilitzar una bateria amb cap dany conegut o visible, incloent-hi fuites o embalums.

Seguir les pautes de temperatura de funcionament que es troben en el manual d'usuari del RPA i de la bateria. Volar en temperatures baixes redueix la capacitat de la bateria i les temperatures altes poden provocar una fallada irreversible.

No utilitzar bateries que hagin entrat en contacte amb aigua. Certes condicions climàtiques, com la boira, poden provocar condensació dins la bateria i el RPA.

Mantenir els connectors de les bateries, carregadors i RPAs lliures de residus i pols. Els connectors es poden netejar amb un drap net i sec o amb un pot d'aire comprimit.

Es recomana repartir l'ús entre múltiples bateries i equilibrar així la pressió que s'exerceix sobre elles. Les bateries estan degudament etiquetades i existeix un registre d'ús que en facilita el monitoratge.

No instal·lar ni retirar mai una bateria d'un RPA quan està encès.

Volar amb la bateria completament carregada i muntada de manera segura al RPA.

Evitar volar el RPA de forma erràtica, incloent-hi canvis sobtats de direcció o frenades brusques, ja que provoca una ràpida descàrrega de la bateria. Intentar mantenir l'operació en moviments constants i frenar lentament durant períodes de vol més llargs.

Si una bateria s'incendia, no utilitzar aigua per apagar el foc, ja que podria provocar que s'incrementi i es propagui. Utilitzar sorra o un extintor dissenyat per incendis elèctrics, com els de pols ABC.

Realitzar una càrrega i descàrrega completa cada 20 cicles, augmentant així el cicle de vida de la bateria. Les bateries LiPo no sofreixen d'efecte memòria, però sí que necessiten alguns procediments d'ajust.

En cas d'error d'una bateria, intentar descarregar-la per complet i tornar a recarregar-la. Les *bateries intel·ligents de DJI* retenen certa càrrega, el que ajuda a evitar errors irreversibles en descarregar-les per complet.

> Les *bateries intel·ligents de DJI* es venen en mode d'hibernació. En utilitzar una bateria nova, s'ha de carregar al 100% per activar-la degudament. Les bateries també entren en mode d'hibernació si s'esgota i s'emmagatzema durant un llarg període de temps.

## Càrrega de Bateries

Utilitzar només carregadors oficials o aprovats pel fabricant.

Carregar les bateries en un ambient controlat, sense humitat i dins del rang de temperatures indicat al manual, generalment entre 22°C i 28°C.

No carregar les bateries just després del seu ús. Deixar refredar les bateries abans de carregar-les.

No carregar les bateries sense supervisió, ni sobre una superfície inflamable. Utilitzar caixes metàl·liques o bosses ignífugues.

Les *bateries intel·ligents de DJI* utilitzen 4 LEDs per indicar el nivell de càrrega.

  | LED1 | LED2 | LED3 | LED4 | Càrrega Bateria |
  | -- | -- | -- | -- | -- |
  | * | * | | | 0% - 50% |
  | * | * | * | | 50% - 75% |
  | * | * | * | * | 75% - 99% |
  | | | | | Càrrega completa |

A més del nivell de càrrega, els 4 LEDs indiquen l'estat de la bateria, incloent-hi la temperatura de càrrega, detecció de curtcircuit, detecció de sobrecàrrega, etc. Aquests indicadors es mostren durant el procés de càrrega.

| LED1 | LED2 | LED3 | LED4 | Estat Bateria |
| -- | -- | -- | -- | -- |
| | 2x * / s | | | Sobrecorrent detectat |
| | 3x * / s | | | Curtcircuit detectat |
| | | 2x * / s | | Sobrecàrrega detectada |
| | | 3x * / s | | Sobrevoltatge carregador detectat |
| | | | 2x * / s | Temperatura càrrega massa baixa < 0 °C |
| | | | 3x * / s | Temperatura càrrega massa alta > 40 °C |

Tot i que les *bateries intel·ligents de DJI* tenen un sistema de seguretat contra sobrecàrregues, és recomanable retirar les bateries un cop el procés de càrrega ha finalitzat.

## Emmagatzematge de bateries

Per a l'emmagatzematge de les bateries s'han d'aplicar diferents protocols, en funció del temps que estaran les bateries sense utilitzar.

**Emmagatzematge a curt termini** Entre 1 i 10 dies. Les bateries s'han de descarregar a un nivell entre 60% i 80%.

**Emmagatzematge a llarg termini** Més de 10 dies. Les bateries s'han de descarregar a un nivell entre 40% i 60%. Les bateries no s'han de deixar mai més de 3 mesos sense utilitzar, ja que redueix considerablement la seva vida útil.

Les bateries s'han d'emmagatzemar en ambients secs, ventilats i mai sota llum directa del Sol. No emmagatzemar la bateria instal·lada en un RPA, ja que una fallada en la bateria podria causar danys a l'aeronau.

Les bateries LiPo són relativament segures, però per augmentar-ne la seguretat es recomana emmagatzemar-les en bosses ignífugues i caixes de metall que puguin contenir un eventual incendi.

No emmagatzemar mai bateries dins de vehicles.

> Les *bateries intel·ligents de DJI* es descarreguen automàticament passat el temps especificat a l'app DJI Go 4.

## Viatjar amb bateries

Transportar les bateries sempre dins de caixes ignífugues específiques i subjectes per evitar que els connectors entrin en contacte amb objectes que puguin provocar un curtcircuit.

La legislació sobre transport de bateries en avions acostuma a ser bastant restrictiva i variable. Revisar que especifiquen tant les normatives locals i internacionals si s'ha de viatjar amb avió.

Seguir les directrius d'emmagatzematge sempre que es viatgi amb bateries.

## Emparellament de Bateries

Alguns models de RPA requereixen dues bateries duals per operar, i aquestes bateries han d'estar emparellades.

L'emparellament de bateries es pot realitzar en qualsevol moment, però es recomana no fer-ho constantment. S'ha d'intentar mantenir sempre les mateixes bateries emparellades.

> La comprovació i emparellament de bateries es realitza des de l'app DJI Go 4, en la secció de configuració de bateries. És recomanable etiquetar les bateries emparellades i utilitzar-les sempre conjuntament.

## Rebuig de bateries

Les bateries LiPo es consideren residus perillosos i no es poden llençar en contenidors estàndard. Les bateries s'han de dur a un centre de residus i reciclatge i dipositar-se al contenidor de bateries de liti.

## App DJI Go 4

L'app DJI Go 4 s'utilitza per controlar la majoria de RPAs de DJI. L'app també permet monitorar l'estat de les bateries i controlar-ne diferents propietats.

### Configuració bàsica

La configuració bàsica permet comprovar el voltatge de la bateria, així com el balanç entre les cel·les, la temperatura, la potència restant, la capacitat total i el nombre de cicles.

La diferència de voltatge entre les cel·les de la bateria no ha de superar els 0.04V. Si aquest valor és excedit, s'ha de retirar la bateria i enviar-la per una inspecció professional.

Es pot modificar les alertes de baixa bateria i bateria crítica, així com activar i desactivar el mode RTH per nivell de bateria.

### Configuració avançada

La configuració avançada permet definir els dies per a que la bateria es descarregui automàticament fins a nivell òptim per emmagatzematge de llarg període.

### Missatges d'alerta

A part de la configuració de paràmetres, l'app mostra també una sèrie d'alertes relacionades amb la bateria.

- **Overcurrent in Discharge** Els motors del RPA estan sol·licitant més potència de la que la bateria pot entregar. Pot ser degut a una baixa temperatura ambiental, vent massa fort, o un pilotatge molt agressiu. Si les causes són ambientals, aturar l'operació fins que aquestes millorin. Realitzar un pilotatge més suau.

- **Over Temperature in Discharge** La temperatura de la bateria és massa alta, i el RPA redueix automàticament la potència dels motors per prevenir danys. Aturar l'operació i avaluar les causes de l'increment de temperatura.

- **Low Temperature in Discharge** La temperatura de la bateria és massa baixa. Aturar l'operació i escalfar la bateria.

- **Cell Damaged** Les cel·les de la bateria no funcionen correctament. S'ha d'aturar immediatament l'operació i entregar la bateria per a la seva inspecció i reparació.

Des del menu `Battery > Advanced Settings > History` es pot veure un historial de les alertes i comprovar si han aparegut amb anterioritat. També es pot revisar l'historial de vols previs per comprovar totes les alertes prèvies.

Les alertes proporcionades per l'app proporcionen informació no detectable a simple vista, i s'han de tenir en compte i ser reportades si convé per augmentar la vida útil de les bateries.

## Annexos

1. [Directrius de seguretat per a bateries intel·ligents DJI Inspire 2](https://dl.djicdn.com/downloads/inspire_2/20170120/INSPIRE+2+Intelligent+Flight+Battery+Safety+Guidelines.pdf)
2. [Directrius de seguretat per a bateries intel·ligents DJI Mavic Air](https://dl.djicdn.com/downloads/Mavic%20Air/Mavic%20Air%20Intelligent%20Flight%20Battery%20Safety%20Guidelines%20v1.0.pdf)
3. [Intelligent Flight Battery Care Guide](https://store-guides2.djicdn.com/guides/wp-content/uploads/2017/07/battery11-1.jpg)
4. [A guide to understanding LiPo batteries](https://rogershobbycenter.com/lipoguide)
