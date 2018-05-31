<h1> Création de suivit du projet de Fran NOVOTNI KASIC </h1>

<ul> <li> Séance numéro 1 (21 décembre 2017) </li>
</br>

<p>Etant un flemmard en ce qu'il s'agit de chercher le courrier, j'ai décidé de créer une boite au lettre connectée qui aura pour but
d'envoyer un message lorsque l'on reçoit du courrier. </br>Il faudra donc utiliser un module de connectivité tel qu'un module WIFI ou Lora (module Lora sera priviligié car le module WIFI cosomme trop d'énergie par rapport à la quantité d'information à transmettre) .</p><br>

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTLZkSWdXVmQdTaTTETlZKux6ojXKBVzKE4rEyHgbqocj2zRL4W" title="Module LORA" align="center" >

</br>

<p>Il faudra également que le message envoyé renseigne si une lettre a été déposé dans la boite au lettre par la fente ou bien si la boite au lettre a dû être ouverte pour y déposer un colis. </p>
</br>

<li> Séance numéro 2 (12 janvier 2018) </li> </ul>
</br>

<p>L'ouverture de la boite au lettre en cas de remise de colis ne se fera plus grâce à une clé mais un système de code. La boite au lettre sera alors fermée par le biais d'un servo moteur, celui-ci controlé grâce à un potentiomètre et le code de la boite au lettre. Lorsque le facteur voudra déposer un colis, il devra tourner le potentiomètre afin d'obtenir une certaine tension nécessaire et rentrer le code. La fermeture de la boite au lettre se fera en remettant le pentotiomètre à sa position initiale.
On mettra également des led qui s'allument en fonction de l'intensité du potentiomètre, et une autre qui clignotera si une lettre ou un colis a été déposé dans la boite au lettre.</p>

<strong> C'est parti </strong>

Récapitulons le matériel nécessaire:
<ol> <li> Une boite au lettre </li>
<li> Des leds </li>
<li> 5 boutons poussoir <strong> ou </strong> 4 boutons poussoir + 1 microrupteur </li>
<li> Un module Lora </li>
<li> Des fils de connection Breadboard </li>
<li> Un potentiomètre </li>
<li> Un servo-moteur + levier de servo</li>
</ol>

<p>D'autres composants pourront être utiliser en fonction de l'avancement du projet.

<strong> Recherche du matériel sur différents sites. </strong></p>
</br>

<ul> <li> Séance numéro 3 (19 janvier 2018) </li>
</br></ul>

<p>Dans cette séance, j'ai fini la la recherche du matériel. J'ai obtenu un servo-moteur à partir du quel je vais créer le premier code de ma boite au lettre. Le servo moteur a un levier unidirectionelle, il servira alors de serrure et remplacera celle qu'on utilisait avec la clé.</p>
<p>Je crée alors un deuxième code qui va permettre l'allumage de trois led en fonction de l'intensité renvoyé par un transistor, il faudra que les trois leds soient allumés avant de taper le code pour que le servo-moteur s'actionne et que la boite au lettre s'ouvre. En fermant la boite au lettre, il suffira de mettre le transistor à son état initial (donc plus de led allumé et servo-moteur à l'état initial)</p>

</br>
<ul> <li> Séance numéro 4 (24 janvier 2018) </li></ul>
</br>

<p>Présentation des projets

<https://github.com/frankasic/Bo-te-au-lettre-connect-e/blob/master/doc/Pr%C3%A9sentation%20Arduino%201.pdf></p>
</br>


<ul> <li> Séance numéro 5 (7 février 2018) </li></ul>
</br>

<p>J'ai fini le codage des leds ainsi que du transistor. Je commence le codage pour le code, j'utiliserai 4 boutons poussoirs qui correspondront chacun à des chiffres (1;2;3, et 4) et qui serviront à taper un code (que l'on aura choisi). Ce code permettra alors l'ouverture de la porte de la boite au lettre, et on pourra la refermer en réactionnant le potentiomètre</p>

</br>
<ul><li> Séance numéro 6 (19 février 2018)</li></ul>
</br>

<p>Lors de cette séance j'ai continué le codage des boutons avec quelques boutons que M. Masson m'a prété en attendant la livraison de ceux que j'avais commandé et qui était un peu différents. De plus j'ai mis en pause le codage de ces boutons car lors de cette séance était venu le module LORA qui permet la communication entre la boite au lettre et le propriétaire de cette dernière. J'ai alors soudé avec l'aide de M.Ferrero le module sur une autre carte Arduino, mais nous avons finalement remarqué en fin de séance que la carte arduino sur laquelle nous avons placé le module LORA n'était pas compatible avec ce dernier et que donc son utilisation n'était plus possible. </p>

</br>
<ul><li> Séance numéro 7 (12 mars 2018)</li></ul>
</br>


<p> Lors de cette séance M.Ferrero m'a apporté une nouvelle carte arduino sur laquelle il avait soudé un module LORA pendant les "vacances".
  J'ai alors pû installer le module et le mettre sur le réseau qu'avait créer M.Ferrero avec sa Gateway, un réseau qui couvre une zone allant des Luciolles aux Templiers. Je met également dans les codes sources, le code que j'ai utilisé pour l'installation du LORA sur ce réseau (code réalisé par M.Ferrero). J'ai alors créer un compte sur The Things Network qui est un réseau fonctionnant grâce à la technologie LORA et sur lequel j'ai enregistré mon appareil, en utilisant un des codes permettant l'installation de mon module avec l'arduino, je remarque sur ce site que le LORA est bien en fonctionnement. Je crée alors un compte Cayenne sur lequel je pourrai visualiser toutes les informations que mon LORA m'enverra. </p>
  
 </br>
<ul><li> Séance numéro 8 (26 mars 2018)</li></ul>
</br>


<p>Présentation des projets

<https://github.com/frankasic/Bo-te-au-lettre-connect-e/blob/master/doc/Pr%C3%A9sentation%20Arduino%202.pdf></p>
</br>
  
  
  
  
 </br>
 <ul><li> Séance numéro 9 (5 avril 2018)</li></ul>
 </br>
 
<p>Lors de cette séance j'ai essayé de modifier le code utilisé pour le LORA afin que j'envoie différentes informations à mon application Cayenne, ça n'a pas été u grand succès car pour renvoyer des informations à l'application, il faut que le code soit écrit d'une certaine manière.</p>

 </br>
 <ul><li> Séance numéro 10 (9 avril 2018)</li></ul>
 </br>
 
 <p> Lors de cette séance j'ai continué de tester différentes façon de codage pour le LORA, j'ai réussi à comprendre comment renvoyer les informations à Cayenne mais cependant il n'est pas possible de renvoyer un texte. J'ai également décidé d'ajouter une led RGB sur la face avant de la boite au lettre qui clignotera en rouge si le code tapé n'est pas le bon et en vert dans le cas contraire. J'ai également dû modifié le codage des boutons en raison d'un problème d'appuie sur un bouton, celui-ci me renvoyer plusieurs fois sa valeur alors que je ne la voulais qu'une seul fois.</p>
 
 </br>
  <ul><li> Séance numéro 11 (2 mai 2018)</li></ul>
 </br>
 
 <p> Lors de cette séance, tout mes codes étant plus ou moins fini, j'ai décidé d'assembler tout les codes, l'ordre étant important j'ai dû changer plusieurs fois l'assemblage du code final. J'ai également reçu une petite batterie qui va permettre d'alimenter mon LORA. En basse consommation, la batterie aura de quoi alimenter le LORA pendant 2 ans. J'ai commencé à assembler ma boite au lettre en fin de séance.</p>
 
 </br>
 <ul><li> Séance numéro 12 (9mai 2018)</li></ul>
 
 <p>C'est la der des der ! Ayant réussi à percer cette satané boite en métal chez moi, je reviens en td pour faire 1h30 de soudage. J'ai également reçu durant la séance une batterie de 9V pour pouvoir alimenter ma carte arduino. En voulant brancher les deux (fil rouge de la batterie au Vin de l'arduino et fil noir au GND) rien ne s'est passé, j'ai réssayé avec une seconde batterie de 9V et toujours rien. J'ai alors décidé d'alimenter mon arduino grâce à la prise usb. De plus je devrai entre la cette dernier séance et la séance de présentation commencer à emboiter le matériel électronique avec la boite puis tout tester dans son ensemble.</p>
 
 </br>
 
 <img src="https://t4.ftcdn.net/jpg/01/57/61/73/240_F_157617369_UgGpLU6dEq1Uh87mFI5OWJx0hA9U2t7N.jpg" title="Merci">
 
 
