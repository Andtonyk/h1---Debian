# H1 - Oma Linux - X-Osio

# Vapaa =/= ilmainen ja ilmainen =/= vapaa!

## Vapaa ohjelmisto,  onko sellaista?

Termillä "Free software" ei tarkoiteta ohjelmaa joka ei voisi maksaa jotakin, vaan ohjelmaa jota voi omissa käsissä vapaasti muokata, kopioida ja käyttää.

Termi ei siis tarkoita samaa asiaa kuin "vapaa lähdekoodi". Vapaalla lähdekoodilla toteutetuissa ohjelmistoissa ei ole "vapaan ohjelmiston" mukaista perusajatusta, joka pohjaisi itseään kollektiivisuuteen ja etiikkaan.
Vapaan lähdekoodin projekti voi täyttää vapaan ohjelmiston mukaiset kriteerit, mutta tämä ei ole taattua tai mitenkään oletettavissa.

## Vapaan ohjelmiston neljä virstaan pylvästä 

- Vapaus käyttää ohjelmistoa miten käyttäjä haluaa ja vapaus tutustua ohjelmiston koodiin sekä sen toimintoihin, rajoituksetta. 
- Vapaus muokata ohjelmaa niin että se toteuttaa ohjelmistollisia toimintoja sinun ohjelmoimallasi tavalla. 
- Vapaus jakaa ohjelmistosta kopioita, ilman erillisien lupien tarvetta.
- Vapaus jakaa alkuperäisestä ohjelmistosta muokattuja versioita eteenpäin, ilman erillisien lupien tarvetta.

Kaikki muokkaamiseen ja muokkaamista edistäviin toimiin, kuten koodiin tutustumiseen liittyvät osioita vaativat että käyttäjällä on vapaa pääsy lähdekoodiin.
Ilman kyseistä eri vapautta, ei ohjelmistoa pystyisi muokkaamaan yhtä jouhevasti tai muokkaamisen helpottavia otteita koodista pääsisi katsomaan.

## Tulisiko vapaan ohjelman astua maksullisuuden varpaille?

Lyhyesti: ei. Pidemmän kautta ei, mutta...: Vapailla ohjelmilla tulee olla mahdollisuus toteuttaa yrityksien- sekä käyttäjien ympäristöihin soveltuvia ohjelmistoja. Isoin kysymys tulee mahdollisien maksullisuuden muotojen analysoinnissa. 
Esimerkiksi IT-ammattilaiselle palkan maksaminen, jotta tämä kehittäisi- tai jatko kehittäisi jotakin ohjelmisto kokonaisuutta voidaan katsoa maksulliseksi, mutta se ei ole vapaan ohjelmiston periaatteiden vastaista. 
Maksullisuus voidaan nähdä vapaata ohjelmistoa vastaisena ideana jos se estäisi vapaan ohjelmiston neljää peruspilaria toteutumasta, muttei tapauksessa jossa maksettua sisältöä saisi jakaa eteenpäin, muokata ja käyttää vapaasti.
Osa kyseistä kokonaisuutta olisi ostetun ohjelmistopaketin logojen ja mahdollisen nimen vaihtaminen ennen sen eteenpäin jakamista. Tästä tosin huomiona että ohjelmiston tulee silti olla ajettavissa nimen muuttamisen jälkeenkin, eli nimen muuttaminen ei saa vaikuttaa 
ohjelmiston kriittisien toimintojen toteutumista estäviksi.

## Yar har dubadidii, onko piratoinnilla ja vapaalla ohjelmistolla jotain yhteistä?

Kyseisillä termeillä ja niihin sidotuilla merkityksillä ei ole mitään tekemistä toistensa kanssa. Vapaa ohjelmisto ei takaa ilmaisuutta ja pyrkii toimimaan ajatusmaailmojen ja etiikan muuttujana. 
Piratismi taas voidaan nähdä enemmänkin henkilön omana ratkaisuna ja vastalauseena jo vallitseviin ajatusmaailmoihin ja niiden ympärille rakennettuihin "eettisiin" toimintamalleihin, mutta se ei itsessään pyri muuttamaan tai muokkaamaan yhteiskuntaa ja sen toimintamalleja.

## Ohjekirja kuuluu pakettiin!

Vapaan ohjelmiston teeseihin kuuluu myös sisällyttää mahdollisen ohjelman lisäksi siihen liittyvä ohjeellinen dokumentaatio, sillä ohjelma ja ohjelman toiminnan kartoittava teksti nähdään erottumattomasti toisiinsa liitetyiksi.

### Lähteet: https://www.gnu.org/philosophy/free-sw.html, Free Software Foundation, Inc. - What is Free Software? / https://www.gnu.org/philosophy/open-source-misses-the-point.html, Richard Stallman - Why Open Source Misses the Point of Free Software

---

# H1 - Oma linux - A-Osio

Tehtävä H1 - Linuxin asentaminen VirtualMachinelle on toteutettu Windows 10 OS:llä, Google Chrome selaimella ja koneena on toiminut Legion 5 kannettava. 16Gt RAM, AMD Ryzen 7 5800H, NVIDIA Geforce 3070 ja 200GB vapaata levytilaa SSD-levyasemalla.

# Alku laukaus Linuxille ja hyvää jatkoa VirtualMachinelle

## Asennusta edeltavät toimet

Aloitin tehtävän kirjoittamalla käyttämääni selaimeen (Google Chrome) opettajan antaman verkkosivun osoitteen "terokarvinen.com".

![terokarvinen com perusnakyma](https://github.com/Andtonyk/h1---Debian/assets/149326156/eff34225-b9b8-47a7-abbb-a42cbb99db61)


Tämän jälkeen jälkeen valitsin sivun navigointipalkeista vaihtoehdon "Courses", eli kurssit, jonka kautta oletin pääseväni alkaneen kurssin sisältöön.
Kursseja oli sivulla useita, joten valitsin niistä nimellisellä tunnisteella osallistumistani vastaavan "Linux Palvelimet 2024 alkukevät".

![terokarvinen com courses](https://github.com/Andtonyk/h1---Debian/assets/149326156/b1e3f466-aa7a-4626-8108-f1affe85d2d8)



Sivulla oli paljon tietoa itse kurssista ja useita linkkejä aineistoihin ja tehtäviin liittyen, tämän tehtävän kannalta tärkeimmät olivat sivua alaspäin mennessä kohdassa linkki "Install Debian on Virtualbox - Updated 2023". 

![terokarvinen com linux info and links](https://github.com/Andtonyk/h1---Debian/assets/149326156/aa83e4d6-a459-4a89-8e03-3786427928c0)

Kyseisen linkin takaa löytyi saman niminen sivu, jossa oli ohjeistukset sekä linkit itse tehtävän toteuttamisen kannalta olennaisiin softiin sekä toimiin.

![VM dl link and debian dl links](https://github.com/Andtonyk/h1---Debian/assets/149326156/a00e4ddf-4445-4d07-b41f-fd115a6ffdcc)




## VirtualMachinen asentaminen koneelle

Aloitin sivun kohdasta "Create a New Virtual Machine" avaamalla kentän linkin " download VirtualBox installer" uuteen välilehteen. 
Linkki ohjasi minut VirtualBoxin omien sivujen lataus-vaihtoehtoihin.

![VM site dl screen](https://github.com/Andtonyk/h1---Debian/assets/149326156/7151c1c5-1c53-4033-b564-c627f5cd5738)

Valitsin näistä uusimmaksi tarjotun vaihtoehdon, joka oli "VirtualBox 7.0.14" käyttöjärjestelmäni ollessa Windows, latasin sille sopivan version. Kyseinen latausvaihtoehto oli oletuksellisesti 64-bittinen, ainakin Windowsille. 

Jos käytössäsi ei ole Windowsia tai jos käyttöjärjestelmäsi vaatii 32-bittisen version, lataa omalle käyttöjärjestelmällesi sopiva versio VM:n lataussivulta.
Onnistuneen latauksen jälkeen avasin tiedoston kansiosta, johon olin sen ladannut.

Asentaminen saattaa vaatia lupaa tietokoneelle tehtävien muutoksien osalta, jos koneen tietoturvassa on asetettu kyseinen varmistus. Tiedostin että olin itse ladannut ohjelman ja asentamassa sitä, joten myönsin sille luvan tehdä muutoksia koneeseeni.
Sitten avautui itse VM:n asennus ikkuna. 

![VM asennus ikkuna](https://github.com/Andtonyk/h1---Debian/assets/149326156/6ffdb35f-c116-414c-999d-f598e4b7b072)

Asennus oli yksinkertainen ja vaati ensin asennuskohdistuksen, jonka valitsemisen jälkeen voi painaa "Next". Itse en tehnyt oletukselliseen tallennuskohteeseen muutoksia.

![VM asennus ikkuna 2](https://github.com/Andtonyk/h1---Debian/assets/149326156/2fee0c6c-b00b-43e3-916c-7a2c5196a16e)

Tämän jälkeen VM-asennus ilmoittaa mahdollisesta tarpeesta VM:n verkosto-osien asennuksen yhteydessä hetkellisesti katkaista verkkoyhteyden, jotta käyttäjä voi ottaa kyseisen mahdollisen katkoksen huomioon muussa koneen käytössä.
Jos mitään sellaista ohjelmaa tai toimintoa ei ole aktiivisena, joka vaatisi katkeamattoman nettiyhteyden voi asennuksen viedä eteenpäin.

![VM asennusikkuna 3](https://github.com/Andtonyk/h1---Debian/assets/149326156/1411c037-252d-4c30-9d8c-628c257e3520)

VM:n asennuksessa kesti itselläni noin minuutti, jonka jälkeen sain onnistuneen asennusilmoituksen ja kysymyksen avataanko VM-ohjelma asennuksen päätyttyä. Itse pidin täpän vaihtoehdossa, joka avasi ohjelman asennuksen päätyttyä.

Kun pystyin todentamaan VM:n toiminnan sen avautumisen ja vetovalikkojen reaktiivisuuksien kautta, siirryin takaisin terokarvinen.com sivulle "Install Debian on Virtualbox - Updated 2023" ja aloitin Linux-paketin lataamisen mahdollistavat toimet.

## Debianin asentaminen koneelle ja VirtualMachille

Vielä sivulla "Install Debian on Virtualbox - Updated 2023" oli aika aloittaa Linux-paketin lataus. 
Tämä oli mahdollista avaamalla sivulla oleva linkki (live amd64 folder on cdimage.debian.org) uuteen välilehteen ja rullaamalla sivua alas, kunnes uusin mahdollinen versio tuli iso-tiedostomuodossa valittavaksi.

![Teros repository site](https://github.com/Andtonyk/h1---Debian/assets/149326156/d319b3b6-e5fd-4544-8e5b-45600c563813)

Ohjelma-paketin lataaminen alkoi klikkaamalla haluttua pakettia. 

![neweast debian version in its iso formet](https://github.com/Andtonyk/h1---Debian/assets/149326156/f616fa15-214c-4435-8e9f-42fbe5bd35cd)

Kyseinen "debian-live-12.4.0-amd64-xfce.iso" oli kooltaan 3 Gt, jonka lataamisessa meni itselläni noin 9 minuuttia.
Onnistuneen latauksen jälkeen kyseinen paketti on mahdollista avata VM:llä, jolloin itse Linuxin asentaminen VM:lle saattoi alkaa.

### Linuxin asentaminen VM:ssä - Ohjelmisto-paketin haku sekä sen virtuaalisien OS-asetuksien määrittäminen

Käynnistin VM:n sen pikakuvakkeen kautta ja ohjelman avauduttua graafiseksi näkymäksi valitsin vaihtoehdon "New". Sen voi myös valita yläpalkin alasvetovalikosta "Machine".

Kyseinen valinta avasi valikko-rakenteen, jossa pääsin muodostamaan tulevaan virtuaaliseen ympäristöön liittyviä valintoja.
Ensiksi oli tärkeää nimetä virtuaalinen ympäristö. Kyseinen nimi on se jolla se listautuu VM:ään.
Samassa näkymässä tulee valita muodostettavan virtuaalikoneen kohde kansio sekä ISO-tiedosto, joka esimerkissämme oli ladattu debian tiedosto. 
Etsin tämän jälkeen debian-pakettini "debian-live-12.4.0-amd64-xfce" siitä polusta, johon olin asettanut sen.
Kun haluttu ISO-paketti oli valittu, OS:n tyyppi (Linux) sekä versio (Debian 64 bit) varmistettu ja "Skip Unattended Install" oli täpättynä, siirryin seuraavaan vaiheeseen kohdassa "Hardware".

![VMssä uuden osin asentamisen valinnat 2-vaihe](https://github.com/Andtonyk/h1---Debian/assets/149326156/ecfdee0e-0a3d-4767-9f9f-e45067c7553d)

### Linuxin asentaminen VM:ssä - Virtuaalikoneen raudallisien asetuksien määrittäminen
VM:n "Hardware" kohta mahdollisti muodostettavan virtuaalisen ympäristön raudalliset rajoitteet RAM:in ja Prosessorien määrien asettamisella. Oletukselliset valinnat olivat liian alhaiset tarpeisiimmme, joten muokkasin prosessorien määrän kahteen ja RAM:in määrän 4000 Mb:hen.
"Enable EFI" kohdan jätin tyhjäksi, sillä debian ei vaatinut sitä onnistuneen asennuksen toteuttamiseksi. Tämän jälkeen siirryin määrittämään virtuaalisen koneen kovalevyllisiä asetuksia kohdasta "Hard Disk".

![VMssä uuden osin asentamisen valinnat 4-vaihe  cpu ja ram muokattu ohjeiden mukaisesti](https://github.com/Andtonyk/h1---Debian/assets/149326156/52710a4b-254c-4d27-ae71-39d692992c27)

### Linuxin asentaminen VM:ssä -Virtuaalikoneen kovalellysien asetuksien määrittäminen

Valitsin vaihtoehdoista "Create a Virtual Hard Disk now" ja aloin toteuttamaan muutoksia.
Oletuksellinen kovalevyn sijainti oli minulle hyväksyttävä, joten en muokannut sitä. 
Kovalevyn tila oli liian rajallinen, joten kasvatin sen koon 60 Gb:hen.
Kovalevyn tyypiksi valitsin VDI:n (VDI - Virtual Disk Image), mutta en valinnut sille tallennuskoollisia variaatioita. Tämän jälkeen viimeistelin uuden virtuaalikoneen valitsemalla kohdan "Finish".

![VMssä uuden osin asentamisen valinnat 5-vaihe  kovalevyn koko, sijainti ja muoto sekä viimeistely](https://github.com/Andtonyk/h1---Debian/assets/149326156/fd18449e-c09c-478e-835e-37455ac4ea49)

## Muodostetun virtuaalikoneen asentaminen VM:ssä

Uusi muodostettava virtuaalikone listautui itselleni Virtual Boxin versiossa 7.0.14 sivun vasempaan laitaan. 
Klikkaamalla haluttua virtuaalikonetta, tulee näkyville sen tiedot, koska nämä olivat itselläni viitteellisissä raameissa, siirryin käynnistämään kyseisen virtuaalikoneen.
Virtuaalikoneen käynnistäminen tapahtuu joko kaksois klikkaamalla haluttua VM:ää, painamalla hiiren oikeaa näppäintä halutun VM:n kohdalla ja valitsemalla avautuvasta valikosta "Start" ja haluttu käynnistys muoto. 
Kolmas tapa käynnistykselle on painaa VM:ssä sen graafisen käyttöliittymän kohtaa "Start" kun haluttu virtuaalikone on valittuna. "Start" vaihtoehdon alasvetovalikosta on mahdollista valita erillisistä käynnistysmuodoista, joita ei tässä kohtaan kuitenkaan tarvittu.

![VM avattu ja silla iso tunnisteellinen debian paketti opettajan sivulta](https://github.com/Andtonyk/h1---Debian/assets/149326156/c8f4d203-831d-4120-8a1d-3521dbe99a8d)

### Linuxin asennus - Käynnistyksen jälkeiset valinnat

Kun haluttu virtuaalikone on startattu, avaa VM uuden erillisen ikkunen sitä varten.
Valitsin vaihtoehdon "Live system (amd64)" painamalla Enter-näppäintä. 


![Muistin vaarin, sehan meni liven kautta  debianin asentaminen](https://github.com/Andtonyk/h1---Debian/assets/149326156/6d636ad9-f880-4751-bbfe-49d9826017ec)

Tämä avasi minulle samassa ikkunassa työpöytä-näkymän, jonka kautta pystyin valitsemaan siinä näkyvän pikakuvake-vaihtoehdon "Install Debian" tupla klikkaamalla sitä.

![Debianin onnistunut live avaus](https://github.com/Andtonyk/h1---Debian/assets/149326156/550ffa4e-5a2f-457d-96d4-140d492932d3)

Tämä käynnisti varoitusilmoituksen epäluotettavasta applikaatio käynnistymisestä, kyseinen ilmoitus on valitettavasti opettajalta saadun tiedon mukaan osa kokonaisuutta, joten valitsin vaihtoehdon "Launch Anyway".

![Debianin asennustoiminnon aktivointi onnistui, vastataan myonteisesti](https://github.com/Andtonyk/h1---Debian/assets/149326156/d43fdd79-80ea-42a9-ab2b-5b6c283d6ff9)

### Linuxin asennus - Muodostettavan Linuxin asetuksien määrittäminen

Asentimen käynnistyttyä pääsin määrittämään asentimen sekä käyttöjärjestelmän kielen kohdassa "Welcome". 
Pidin tämän oletuksellisessa vaihtoehdossa "American English" ja valitsin  "Next".

![Ensi nakyma](https://github.com/Andtonyk/h1---Debian/assets/149326156/9af2a56f-8177-4da0-b72d-6e7685d5ea1c)

Tämän jälkeen pääsin määrittämään alue- sekä aikavyöhykkeitä kohdassa "Location". 
Valitsin alueen jolla toimin, käyttäen kartan valintarakennetta ja klikkaamalla Suomea. Tämä muutti kohdat "Region" ja "Zone" sisällöt vastaamaan seuraavia "Europe" ja "Helsinki". 
Alue- ja aikavyöhykkeiden oltua paikkaansa pitävät, valitsin "Next".

![Sijainti - toinen nakyma](https://github.com/Andtonyk/h1---Debian/assets/149326156/65be1b35-7ef4-4bf9-b210-f1c390e5043f)

Kohdassa "Keyboard" määritin näppäimistölleni sen perusasetukset. Valitsin "Keyboard model" kohdassa vaihtoehdon "Generic 105-key PC".
Näppäimistön kielikenttä asetuksissa valitsin "Finnish" ja alatyypiksi "Default".
Tämän jälkeen valitsin "Next".

![Nappaimisto - kolmas nakyma](https://github.com/Andtonyk/h1---Debian/assets/149326156/a6c5ac54-08fe-4940-855e-528c96974627)

Kohdassa "Partitions" valitsin BIOS-tietojen kohteen, tämän asetin samaksi kuin virtuaalikoneeni kovalevyn sijainnin.
Valitsin kovalevyn tietoja koskevista vaihtoehdoista "Erase disk"
Bootloaderin sijainniksi varmistin saman kuin BIOS-tietojen kohteen, ja varmistin että kohta "Encrypt system" ei ollut valittuna.
Tämän jälkeen valitsin "Next".

![Kovalevyn ositus - neljas osio](https://github.com/Andtonyk/h1---Debian/assets/149326156/631e268d-4330-4da4-8443-b85351553747)

Kohdassa "Users" syötin etu- sekä sukunimeni kenttää "What is your name?".
Muodostin itselleni käyttäjätunnuksen syöttämällä käytettävän nimen (andreask) kenttään "What name do you want to use to log in?".
Nimesin koneeni Ulthweksi kentässä "What is the name of this computer?".
Lisäsin itselleni salasanan syöttämällä kohdassa "Choose a password to keep your account safe" alla oleviin kahteen kenttään identtisesti.
En täpännyt vaihtoehtoa "Log in automatically without asking for the password".
Tämän jälkeen valitsin "Next".

![Kayttaja - viides osio](https://github.com/Andtonyk/h1---Debian/assets/149326156/85ed8f19-345a-4f3d-ba40-dde7b1002b2d)

Kohdassa "Summary" oli listattuna aiemmin syöttämäni tiedot. Jotta sain näkyville vaihtoehdon "Install" valitsin ruudun oikeassa yläkulmassa näkyvän sivun suurentamisen ikonin.
Tietojen tarkistamisen jälkeen valitsin vaihtoehdon "Install".

![Koonti - kuudes osio](https://github.com/Andtonyk/h1---Debian/assets/149326156/5ee24a44-ce1e-4741-af81-58a1c14f2aa1)

Kohdassa "Install" tuli näkyville asennuspalkki, joka kertoi prosentteina asennuksen etenemisestä tässä meni minun kohdallani noin 5 minuuttia.
Asennuksen valmistuttua näkymä siirtyy automaattisesti viimeiseen kenttään "Install".

![Asennus aloitettu](https://github.com/Andtonyk/h1---Debian/assets/149326156/ab5e1d55-1d0d-4f51-bf94-3b9cb62d5136)

Kohdassa "Finish" asennin ilmoittaa uudelleen käynnistyksen tarpeesta, jonka toteutin automaattisesti jättämällä täpän kohtaan "Restart now" ja valitsemalla tämän jälkeen "Done".

![Asennuksen onnistumisen näkymä](https://github.com/Andtonyk/h1---Debian/assets/149326156/47c3b1d7-11d4-4b24-a019-d8598db72901)

Uudelleen käynnistyksen jälkeen näkymä uudelleen käynnistyy sisäänkirjautumisen näkymään. Syötin tässä aiemmin muodostamini käyttäjätunnuksen sekä salasanan ja valitsin "Log In".

![Sisaankirjautumisen testaus](https://github.com/Andtonyk/h1---Debian/assets/149326156/1b7d8eb9-0431-4fd5-93c6-5c00340b9046)

Virtuaalikone avautui käyttöjärjestelmän mukaiseen työpöytä-näkymään, jonka jälkeen avasin firefoxin ja syötin selaimen url-kenttään "terokarvinen.com". 
Sivu avautui ongelmitta, joka tarkoitti että virtuaalisen koneeni verkkoyhteys toimi ja pystyin ilmoittamaan testini onnistuneesti suoritetuksi.

![Sisaankirjautuminen toimi ja samoin verkko](https://github.com/Andtonyk/h1---Debian/assets/149326156/f2baf909-015d-4b75-a84a-280665e071f4)

### Lähteet: https://terokarvinen.com/, Tero Karvinen / https://www.virtualbox.org/wiki/Downloads, Oracle / https://www.debian.org/, Software in the Public Interest, Inc
