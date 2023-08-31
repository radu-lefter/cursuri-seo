---
layout: ../../layouts/MarkdownPostLayout.astro
title: 'Ghidul SEO pentru programatori'
pubDate: 2023-07-10
description: 'Este un lucru foarte bun cand tot mai multi programatori, si o parte tot mai mare a CMS-urilor, pun baza optimizarii site-urilor pentru motoarele de cautare, inca de la construirea lor.

Deoarece e mult mai greu sa repari astfel de lucruri tehnice cand site-ul a inceput sa primeasca vizitatori, decat daca s-ar asigura o buna accesibilitate si arhitectura a site-ului chiar de la inceput.

De aceea, in acest scurt ghid vom prezenta cateva lucruri pe care ne-am dori ca toti programatorii sa le cunoasca si sa le respecte la construirea site-urilor: un cod al bunelor practici pentru SEO.'
author: 'Ela Iliesi-Visan'
image:
    url: '/images/Ghid-SEO-programatori.png'
    alt: 'ghid-seo'
tags: ["seo", "ghid", "programatori"]
---

# 1. Meta taguri unice si descriptive

Incepem cu a atrage atentia asupra meta tagurilor paginilor, si in special a meta titlurilor, care au o importanta deosebita, deoarece reprezinta paginile site-ului in rezultatele motoarelor de cautare (dar si in social media), influentand numarul de clickuri pe care le vor primi - un factor foarte important pentru SEO.

Desi programatorul nu este obligat sa preia si atributiile unui specialist SEO si sa faca cercetari complexe de cuvinte cheie sau sa creeze titlurile si descrierile cele mai atragatoare pentru utilizatori, acesta poate ajuta la optimizarea paginilor, creandu-le metataguri unice si descriptive.

Exemple de titluri care trebuie evitate:

    `<title>Home</title>`
    `<title>Brand.ro</title>`
si alte titluri prea generale, fara relevanta sau prea lungi.

Programatorul mai poate de asemenea sa creeze un sistem de administrare al continutului site-ului, care sa permita editorilor sa introduca si sa modifice meta tagurile, sau care sa le creeze automat (de exemplu in cazul magazinelor online cu mii de produse, unde acestea pot fi create automat, dupa diverse formule, stabilite de comun acord cu specialistul SEO).

# 2. Fiecarei pagini sa ii corespunda un singur URL

Din fericire, in ultimii ani, intalnim tot mai rar site-uri care au mai multe adrese pentru pagini, precum seria din exemplu de mai jos, unde toate adresele prezentate pot reprezenta pagina principala a site-ului:

    http://www.site.ro
    http://site.ro
    http://www.site.ro/index.php

Si totusi nu exista curs la care sa nu fie cel putin una sau doua persoane cu aceasta problema la site. Problema apare din faptul ca fiecare adresa reprezinta pentru motoarele de cautare o pagina diferita, cu recomandari diferite, iar autoritatea pe care ar putea-o castiga pagina principala a unui site, este impartita intre versiunile de URL existente. In plus continutul adreselor suplimentare poate fi considerat continut duplicat, lucru ce va afecta indexarea site-ului de catre roboti si pozitionarea lui in motoarele de cautare.

O solutie buna o reprezinta setarea unor redirecturi 301 de la adresele suplimentare spre cea care se doreste a fi principala (daca este vorba de un site nou), sau spre acea pagina pe care specialistul SEO a indentificat-o ca fiind cea mai populara / cu cea mai mare autoritate (daca este un site cu vechime). Se mai poate folosi si rel="canonical"daca nu se poate face redirectarea.

# 3. Viteza de incarcare

Odata atrasi pe site, viteza de incarcare ii poate face pe vizitatori sa ramana si sa descopere continutul site-ului sau sa iasa de pe el. De aceea viteza a ajuns unul din factorii SEO, iar pozitia site-urilor in rezultatele motoarelor de cautare este corelata cu viteza de incarcare - mai specific cu time-to-first-byte (TTFB), timpul necesar ca browserul sa incarce primul bit al paginii.

Daca se intampla des ca vizitatorii sa paraseasca site-ul la mai putin de 5 secunde dupa ce au intrat pe o pagina, si se intorc la pagina de rezultate Google pentru a accesa alt site, acest lucru va fi un semnal negativ si va afecta pozitia site-ului in rezultatele motorului de cautare.

Cele mai comune probleme (si lucrurile de avut in vedere) care conduc la o viteza mica de incarcare a paginilor sunt: imaginile neoptimizate, continutul servit necomprimat, nefolosire sprite-uri (CSS), lipsa cache, aglomerarea de plugin-uri, gazduirea slaba. Cu unelte ca Google PageSpeed Insights se poate vedea ce trebuie imbunatatit la anumite pagini. Un scor de peste 70-80 din 100, reprezinta o viteza buna.

# 4. Pagina 404 personalizata

Un alt motiv pentru care vizitatorii vor parasi site-ul sunt paginile de eroare necustomizate. Paginile 404 pot fi gasite in Search Console (Google Webmaster Tool) sectiunea Crawl Errors, sau cu unelte specifice care identifica linkurile site-ului care nu mai functioneaza (brokenlinkcheck.com).

O pagina customizata 404 ajuta atat la SEO cat si la experienta vizitatorilor si indeplinirea obiectivelor site-ului. Spre deosebire de o pagina obisnuita Not found, o pagina 404 personalizata ar trebui sa contina headerul si footerul obisnuit al site-ului, mesajul ca pagina cautata nu mai este disponibila, linkuri spre pagini asemanatoare sau populare, si o casuta de cautare pentru ca utilizatorul sa poata gasi informatia pe care o cauta.

O alta solutie o reprezinta redirectul 301 de la pagina care nu mai este disponibila spre una care o inlocuieste, salvand astfel autoritatea castigata de acea pagina.

A nu se uita si crearea unor pagini customizate 404 optimizate pentru mobil.

# 5. Coduri de urmarire

Ce metataguri sunt duplicate, prea scurte sau prea lungi, care este continutul apreciat al site-ului si ce pagini "gonesc" vizitatorii, care sunt paginile care dau erori sau care se incarca foarte greu.. toate aceste lucruri mentonate pana in aceasta parte a ghidului, si mult mai multe se gasesc rapid folosind unelte ca Google Analytics si Search Console.

De aceea am dori ca toti programatorii sa considere un lucru de la sine inteles faptul ca inainte de predarea unui site sau unei pagini noi, aceasta trebuie sa contina codurile generale si specifice de monitorizare (de exemplu Analytics Ecommerce Tracking code in cazul magazinelor online).

Si daca vorbim de bune practici, am intalnit multi cursanti care nu puteau accesa contul de Analytics deoarece nu stiau adresa si parola, detinute de programator, sau aveau acces limitat la vizualizarea datelor si nu isi puteau seta obiective. Adresa de Gmail care sa stea la baza conturilor trebuie ceruta proprietarului site-ului, impreuna cu parola aleasa de acesta.

# 6. Sitemap XML

Crearea unui fisier sitemap XML ajuta motoarele de cautare sa descopere mai repede paginile site-ului. In functie de marimea si tipul site-ului pot fi necesare si alte fisiere ca:

Video Sitemap
Image Sitemap
Article Sitemap
Mobile Sitemap

Limita unui fisier sitemap este de 50,000 URL-uri, dar se pot adauga mai multe fisiere pentru a se acoperi toate URL-urile site-uui. Nu exista o limita la cate pagini poate indexa Google unui site.
Pentru a genera sitemap-uri se pot folosi plugin-uri sau site-uri ca www.xml-sitemaps.com, iar fisierul trebuie adaugat la adresa http://site.ro/sitemap.xml. Dupa aceea se merge in Google Search Console, sectiunea Crawl - Sitemaps, si se adauga sitemap-urile, cate unul pe rand, folosind butonul Add/Test Sitemap.

Sitemap-ul va contine prioritati si alte informatii care trebuie setate in functie de continutul si importanta paginilor, sau cu ajutorul specialistului SEO.


# 7. Optimizare pentru mobil

Asa cum se poate observa in Search Console sau testand site-ul cu unealta https://www.google.com/webmasters/tools/mobile-friendly/, Google poate verifica usor daca un site este sau nu optimizat pentru mobil. Nu a fost deci un lucru dificil sa adauge acest factor in algoritm si incepand cu 21 aprilie 2015 au si facut-o.

Asa cum au spus in anuntul oficial: “Daca paginile site-ului nu sunt optimizate pentru mobil, se pot inregistra scaderi semnificative in traficul primit din cautarile Google. Dar odata ce site-ul va deveni mobile-friendly, vom reprocesa paginile.”

Pentru a vedea cat de urgenta este optimizarea site-ului pentru mobil, se intra in Analytics, sectiunea Behaviour si se analizeaza comportamentul celor care viziteaza site-ul de pe mobil - este considerabil mai mic numarul de obiective indeplinite, timpul petrecut pe site etc? Atunci trebuie luate masuri rapid.

Site-urile se pot optimiza pentru mobil prin: responsive design (optiunea preferata, asigurand un design bun indiferent de dispozitivul folosit), sau creand URL-uri separate pentru vizitatorii care vin de pe mobil (care vor necesita insa un set nou de optimizari, dar care pot ajuta prin linkuri spre site-ul principal).

# 8. Microformatarea si structurara datelor

Daca pe langa lucrurile pe care suntem obisnuiti sa le vedem in rezultatele motoarelor de cautare, descoperim uneori si diverse informatii suplimentare: precum stelutele primite de un produs, imagini ale produsului, sau chiar casuta de cautare a unui site care apare chiar in rezultatele Google, aceste lucruri sunt posibile datorita microformatarii si structurarii datelor.

Sunt o multime de informatii ce pot fi "explicate" prin microformatare astfel incat motorul de cautare sa poata returna rezultate mai interesante pentru utilizatori, unelte prin care programatorii pot testa codul imbunatatit astfel, si site-uri cu exemple de formatari in functie de tipul site-ului la care se lucreaza.

Aceste lucruri reprezinta doar o mica parte din lucrurile tehnice care trebuie cunoscute de programatori si cei care vor sa optimizeze site-uri. Nu am discutat despre: structura site-ului, structura URL-urilor, optimizarea imaginilor, fisierul Robots.txt, tipurile de pop-ups si cookies ce pot fi folosite, atributul no follow, Rel next si prev, optimizarea site-urilor internationale, noutatile SEO aduse de HTML5, headings, breadcrumbs, alte tipuri de redirecturi..

# Invata mai mult

Pentru aprofundare va recomandam cursurile de SEO de la sediu sau online. Data urmatoarelor cursuri poate fi gasita in formularul de inscriere de pe acest site. Ocupa din timp locul dorit.

Spor la optimizare!
