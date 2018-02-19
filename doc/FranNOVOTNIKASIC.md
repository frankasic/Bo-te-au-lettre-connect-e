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
</br>

<p>Dans cette séance, j'ai fini la la recherche du matériel. J'ai obtenu un servo-moteur à partir du quel je vais créer le premier code de ma boite au lettre. Le servo moteur a un levier unidirectionelle, il servira alors de serrure et remplacera celle qu'on utilisait avec la clé.</p>
<p>Je crée alors un deuxième code qui va permettre l'allumage de trois led en fonction de l'intensité renvoyé par un transistor, il faudra que les trois leds soient allumés avant de taper le code pour que le servo-moteur s'actionne et que la boite au lettre s'ouvre. En fermant la boite au lettre, il suffira de mettre le transistor à son état initial (donc plus de led allumé et servo-moteur à l'état initial)</p>

</br>
<ul> <li> Séance numéro 4 (24 janvier 2018) </li>

Présentation des projets

<ul> <li> Séance numéro 5 (7 février 2018) </li>

J'ai fini le codage des leds ainsi que du transistor. Je commence le codage pour le code, j'utiliserai 4 boutons poussoirs qui correspondront chacun à des chiffres (1;2;3, et 4) et qui serviront à taper un code (que l'on aura choisi).
