Aspecte generale cu privire la codul sursa:
 -comentariile se refera la sectiunea de sub comentariu si descriu in linii mari felul in care programul functioneaza
 -nu am testat daca memoria este sau nu alocata corect folosind e secventa de tipul(if(adr_pointer_malloc != NULL)) deoarece enuntul
 temei nu a specificat daca este sau nu necesar, in cazul in care memoria nu ar fi fost alocata, atunci nu as fi putut printa un mesaj
 sau oprii executia programului deoarece enuntul nu specifica aceasta situatie
 -am folosit local variabile cu nume scurt pentru a retine valoarea unei variabile cu nume lung pentru a creea un cod cat mai 
 aerisit cu putinta ce respecta conventia de coding style, dar in acelasi timp ofera nume de variabile sugestive oricarui cititor
 -comentariile sunt realizate in limba romana, iar numele variabilelor in limba engleza

Aspecte cu privire la alocarea dinamica a memoriei:
  -am ales sa aloc si sa dezaloc cate un element la fiecare introducere in memorie a unui filtru sau a unei imagini, mergand intr-un
  fel din aproape in aproape, deoarece am considerat ca o dublare a memoriei alocate de fiecare data cand memoria curenta se umple sau o 
  injumatatire a acesteia cand jumatate este libera, desi mai eficienta ar fi necesitat retinerea numarului de spatii libere 
  din vectori, complicand codul pentru a realiza o eficientizare a timpului de executie nespecificata in enuntul temei
  -am construit cateva functii auxiliare ce aloca si dezaloca memorie, aceste fiind folosite pentru a nu scrie acelasi tip de alocare/
  dezalocare in mai multe secvente ale codului

Realizarea functiilor de la task-utile 1-6:
  -am explicat felul in care acestea functioneaza comentand codul sursa
  -am ales sa aloc matrici noi in functiile ce modifica dimensiunile acestora, functiile returneaza adresa noii matrici si o sterg pe 
  cea veche
  -formulele au fost concepute cu "creionul si foaia" pornind de la un caz particular cu matrici de dimensiuni mici

Realizarea task-ului interactiv 7:
  -am ales sa folosesc un loop infinit utilizand while(1), iar comenzile au fost implementate folosind functiile create in task-urile
  1-6, cu exceptia celor de exit, load, save, create filter, delete filter si delete image ce sunt scrise direct in main()

Concluzii finale:
 -am utilizat doar informatiile din tematica: functii, vectori, matrici si alocare dinamica, evitand sa folosesc un struct pentru 
 matricea asociata unei imagini si matricea asociata unui filtru
 -conceptul a fost dupa parerea mea unul interesant si captivant, tema prezinta o aplicatie practica a conceptelor din tematica 
 prevazuta, fapt ce ii sporeste valoarea sa de instrument educational 