# 10-Grahlix-29
# OSINT Exercise

#### Piattaforma: Grahlix
#### Livello: Hard/Medium/Hard
#### Date: 2026/01/30
#### Link: https://gralhix.com/list-of-osint-exercises/osint-exercise-029/

## Obiettivo
### 1. Uncover what the person in front of me was reading.
### 2. Identify the train model.
### 3. Identify my seat number.

## Informazioni iniziali
#### - I took the photo below whilst riding a train in the UK. I always prefer quiet areas where no one can sit behind me because, in a public space, no information is truly private.
- ![ss01.png](Media/ss01.png)

## Strumenti usati
-

## Passaggi
1. Ok iniziamo dalla seconda, sappiamo che è negli UK che ce l'ha detto lei, vediamo se ha lasciato i metadati nell'immagine con Exif Viewer, ovviamente li ha tolti :)
2. Su wikipedia https://en.wikipedia.org/wiki/Rail_transport_in_Great_Britain c'è questa tabella di treni ad alta velocità: [High speed trains in Britain](Media/High_speed_trains_in_Britain.md), potrei guardarli uno a uno 
3. Provo una ricerca per immagini specifica: ![[ss02.png]] si trova questo articolo: https://philiphaigh.co.uk/2021/09/when-will-passengers-return/ con questa immagine: ![[ss03.png]] il sedile sembra quello anche se l'adesivo è diverso ma l'immagine dell'articolo è stata scattata nel 2021 quindi ci sta. Cerchiamo di capire il resto del treno
4. I cuscini sono dello stesso colore
5. La barar in alto è di un colore diverso, le cappelliere potrebbero essere simili. Quindi direi che i sedili sono gli stessi sicuro ma sul treno non si capisce bene. Vediamo se si riesce a capire che modello di sedile è e dove viene usato
6. Facendo la ricerca per immagini specifica dei sedili: ![[ss04.png]] troviamo vari riferimenti a treni LNER:
	1. https://x.com/KevinStewartSNP/status/1985413231284756751 LNER service da abeerdeen a edinburgh postata il 3 novembre 2025, in questo caso pare che anche lo sticker sia uguale: ![[ss05.png]] stesso problema che la parte alta è rossa mentre nella foto iniziale sembra grigia
	2. Short di youtube: https://www.youtube.com/shorts/DIWMwUKV-Dc ==LNER azuma== announcement 4 aprile 2025, sempre barra in alto rossa
	3. https://www.facebook.com/groups/dullmensclub/posts/1133870970602776/ post di facebook di novembre 22 in cui si lamenta della gente che parla al telefono e dice che va da York a Kings Cross (Londra), sempre barra in alto rossa
	4. https://tothetrains.uk/lner-class-801-azuma-overview/ Qui c'è una foto dell ==LNER Azuma 801== standard class interno, è del 2021
	5. Qui ![[ss06.png]] conferma che è un LNER (da notare che se sei in una priority seat lo scrivono e lì nel sedile davanti non c'è scritto)
7. Ok sembra evidente che sia un **LNER Azuma 801**, cerchiamolo su google per vedere se risolviamo il problema della barra grigia e troviamo altre info sul posto (BTW, c'è nell'elenco di wiki di prima)
8. https://en.wikipedia.org/wiki/British_Rail_Class_801 qui ci sono molte info e in particolare un link a questo pdf: ![[LNER2710_Azuma_Seat_Maps_Update_V3.pdf]]
9. Considerando che non ha nessuno dietro (lo ha scritto) è in standard class e il sedile davanti non è priority per esclusione l'unico posto possibile è **Coach G seat 6**: ![[ss07.png]]
10. In realtà la parte rossa c'è: ![[ss08.png]]
11. Per rispondere alla 1 specchio l'immagine e faccio zoom: ![[ss09.png]]
12. Si riconoscono alcune parole o sequenze: "long" "have seen better days" "gloves" "portmanteau" (?) "whistle" "she has the" "William's cousin"
13. Cercando su google (NON duckduckgo) si trova qui: https://readfrom.net/sara-sheridan/page,2,629675-the_fair_botanists.html ![[ss10.png]]
14. Il pezzo è questo: *She runs her palms up her arms to smooth her long, unlined tan leather gloves that have seen better days and pats her portmanteau. A long, shrill whistle sounds on deck. She has the letters from William’s cousin, James, in her reticule and now that she is close to meeting him, she feels both nervousness and relief. She will be safe. Provided for at last.*
15. Il libro è **The Fair Botanist, Sara Sheridan**
## Evidenze
- Link:
- Note:

## Risultato / Flag
#### 1. The Fair Botanist, Sara Sheridan
#### 2. LNER Azuma 801
#### 3. Coach G, seat 6
