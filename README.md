Tehtävä H1 - LInuxin asentaminen VirtualMachinelle on toteutettu Windows 10 OS:llä, Google Chrome selaimella ja koneena on toiminut Legion 5 kannettava. 16Gt RAM, AMD Ryzen 7 5800H, NVIDIA Geforce 3070 ja 200GB vapaata levytilaa SSD-levyasemalla.

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

![]()

Oletuksellinen kovalevyn sijainti oli minulle hyväksyttävä, joten en muokannut sitä. Kovalevyn tila oli liian rajallinen, joten kasvatin sen koon 50 Gb:hen.
Kovalevyn tyypiksi valitsin VDI:n (VDI - Virtual Disk Image), mutta en valinnut sille tallennuskoollisia variaatioita. Tämän jälkeen viimeistelin uuden virtuaalikoneen valitsemalla kohdan "Finish".

## Muodostetun virtuaalikoneen asentaminen VM:ssä

Uusi muodostettava virtuaalikone listautui itselleni Virtual Boxin versiossa 7.0.14 sivun vasempaan laitaan. Klikkaamalla haluttua virtuaalikonetta, tulee näkyville sen tiedot, koska nämä olivat itselläni viitteellisissä raameissa, siirryin käynnistämään kyseisen virtuaalikoneen.
Virtuaalikoneen käynnistäminen tapahtuu joko kaksois klikkaamalla haluttua VM:ää, painamalla hiiren oikeaa näppäintä halutun VM:n kohdalla ja valitsemalla avautuvasta valikosta "Start" ja haluttu käynnistys muoto. 
Kolmas tapa käynnistykselle on painaa VM:ssä sen graafisen käyttöliittymän kohtaa "Start" kun haluttu virtuaalikone on valittuna. "Start" vaihtoehdon alasvetovalikosta on mahdollista valita erillisistä käynnistysmuodoista, joita ei tässä kohtaan kuitenkaan tarvittu.

### Linuxin asennus - Käynnistyksen jälkeiset valinnat

Kun haluttu virtuaalikone on startattu, avaa VM uuden erillisen ikkunen sitä varten.
Valitsin vaihtoehdon "Live system (amd64)" painamalla Enter-näppäintä. 
Tämä avasi minulle samassa ikkunassa työpöytä-näkymän, jonka kautta pystyin valitsemaan siinä näkyvän pikakuvake-vaihtoehdon "Install Debian" tupla klikkaamalla sitä.
Tämä käynnisti varoitusilmoituksen epäluotettavasta applikaatio käynnistymisestä, kyseinen ilmoitus on valitettavasti opettajalta saadun tiedon mukaan osa kokonaisuutta, joten valitsin vaihtoehdon "Launch Anyway".

### Linuxin asennus - Muodostettavan Linuxin asetuksien määrittäminen

Asentimen käynnistyttyä pääsin määrittämään asentimen sekä käyttöjärjestelmän kielen kohdassa "Welcome". 
Pidin tämän oletuksellisessa vaihtoehdossa "American English" ja valitsin  "Next".

![]()

Tämän jälkeen pääsin määrittämään alue- sekä aikavyöhykkeitä kohdassa "Location". 
Valitsin alueen jolla toimin, käyttäen kartan valintarakennetta ja klikkaamalla Suomea. Tämä muutti kohdat "Region" ja "Zone" sisällöt vastaamaan seuraavia "Europe" ja "Helsinki". 
Alue- ja aikavyöhykkeiden oltua paikkaansa pitävät, valitsin "Next".

![]()

Kohdassa "Keyboard" määritin näppäimistölleni sen perusasetukset. Valitsin "Keyboard model" kohdassa vaihtoehdon "Generic 105-key PC".
Näppäimistön kielikenttä asetuksissa valitsin "Finnish" ja alatyypiksi "Default".
Tämän jälkeen valitsin "Next".

![]()

Kohdassa "Partitions" valitsin BIOS-tietojen kohteen, tämän asetin samaksi kuin virtuaalikoneeni kovalevyn sijainnin.
Valitsin kovalevyn tietoja koskevista vaihtoehdoista "Erase disk"
Bootloaderin sijainniksi varmistin saman kuin BIOS-tietojen kohteen, ja varmistin että kohta "Encrypt system" ei ollut valittuna.
Tämän jälkeen valitsin "Next".

![]()

Kohdassa "Users" syötin etu- sekä sukunimeni kenttää "What is your name?".
Muodostin itselleni käyttäjätunnuksen syöttämällä käytettävän nimen (andreask) kenttään "What name do you want to use to log in?".
Nimesin koneeni Ulthweksi kentässä "What is the name of this computer?".
Lisäsin itselleni salasanan syöttämällä kohdassa "Choose a password to keep your account safe" alla oleviin kahteen kenttään identtisesti.
En täpännyt vaihtoehtoa "Log in automatically without asking for the password".
Tämän jälkeen valitsin "Next".

![]()

Kohdassa "Summary" oli listattuna aiemmin syöttämäni tiedot. Jotta sain näkyville vaihtoehdon "Install" valitsin ruudun oikeassa yläkulmassa näkyvän sivun suurentamisen ikonin.
Tietojen tarkistamisen jälkeen valitsin vaihtoehdon "Install".

![]()

Kohdassa "Install" tuli näkyville asennuspalkki, joka kertoi prosentteina asennuksen etenemisestä tässä meni minun kohdallani noin 5 minuuttia.
Asennuksen valmistuttua näkymä siirtyy automaattisesti viimeiseen kenttään "Install".

![]()

Kohdassa "Finish" asennin ilmoittaa uudelleen käynnistyksen tarpeesta, jonka toteutin automaattisesti jättämällä täpän kohtaan "Restart now" ja valitsemalla tämän jälkeen "Done".

![]()

Uudelleen käynnistyksen jälkeen näkymä uudelleen käynnistyy sisäänkirjautumisen näkymään. Syötin tässä aiemmin muodostamini käyttäjätunnuksen sekä salasanan ja valitsin "Log In".

![]()

Virtuaalikone avautui käyttöjärjestelmän mukaiseen työpöytä-näkymään, jonka jälkeen avasin firefoxin ja syötin selaimen url-kenttään "terokarvinen.com". 
Sivu avautui ongelmitta, joka tarkoitti että virtuaalisen koneeni verkkoyhteys toimi ja pystyin ilmoittamaan testini onnistuneesti suoritetuksi.

![]()
