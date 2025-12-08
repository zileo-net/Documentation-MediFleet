# La facturation électronique (Peppol)

Obligation légale à partir du 1er janvier 2026, pour les factures (et notes de crédit) à destination **des entreprises européennes assujetties à la TVA**, 
MediFleet vous permet d'envoyer vos factures via le réseau européen _Peppol_. Pour information, cela couvre aussi le cas des institutions qui voudraient 
recevoir leur facture via le portail _Mercurius_ ; l'envoi via Peppol aura le même effet.

## Pré-requis / Activation
Pour pouvoir activer cette fonctionnalité, notre service support doit d'abord créer un profil à votre nom et avec les coordonnées de votre société chez notre 
prestataire de liaison avec le réseau Peppol. (1 profil par profil de facturation configuré sur votre serveur MediFleet.) 
**Une fois cette opération effectuée,** vous serez averti par e-mail, vous aurez accès aux fonctionnalités décrites ci-dessous, et vous pourrez à tout moment
consulter ce que nous avions enregistré comme profil sur un nouvel onglet "Facturation électronique" dans vos <a href="/Configuration/edit?tabIndex=7&menuIndex=1">paramètres généraux</a>.

## Envoi des factures
À partir du moment où vous indiquez que l'une de vos institutions doit recevoir des factures électroniques (ce qui sera expliqué au paragraphe suivant), 
l'envoi des factures est extrêmement simple... Puisqu'il fonctionne de la même manière que l'envoi par e-mail. La seule différence, utile à avoir en tête, 
c'est qu'ici le numéro d'entreprise (n° BCE) sert d'identifiant (d'adresse e-mail en quelques sortes). Vos factures à envoyer vers une telle institution 
se retrouveront dans un onglet "À envoyer via Peppol", qui listera vos factures en attente d'envoi vers ce réseau, et il vous suffira de cliquer sur : 

<button class="ui brown button">Envoyer vers Peppol</button>

Le suivi des envois (réussite ou erreur), apparaîtra alors dans le suivi de la facture, tout comme les envois par email. En cas d'erreur sur une facture, celle-ci se retrouvera dans l'onglet "Erreur d'envois Peppol".

> À noter : Nous n'envoyons pas la facture en parallèle par e-mail pour éviter tout double encodage du côté des institutions ; en théorie, il est de la responsabilité des logiciels qui réceptionnent des factures de Peppol de prévenir qui de droit.

## Gestion des institutions
Pour pouvoir envoyer une facture électronique à une institution, il faut que celle-ci se soit enregistrée sur le réseau Peppol, en indiquant qu'elle accepte de recevoir 
certains types de document. Nous sommes en mesure de détecter ces enregistrements. Nous le faisons automatiquement chaque nuit. Ce qui donne, pour chaque institution cliente, 
4 statuts possibles : 

- <i class="red times icon"></i> Non enregistrée sur le réseau Peppol
- <i class="red times circle outline icon"></i> Enregistrée mais n'acceptant pas les documents envoyés par MediFleet
- <i class="yellow check icon"></i> Enregistrée, vous pouvez activer les envois de factures électroniques
- <i class="green check icon"></i> Envois via Peppol activés pour cette institution

Cette information est disponible dans une nouvelle colonne de votre liste d'institutions clientes. Nous n'activons pas automatiquement les envois, 
nous préférons que vous puissiez choisir d'activer où non cette nouvelle méthode ; même si elle devient obligatoire à partir du 1er janvier 2026. 
Pour ce faire, vous trouverez sur chaque profil d'institution un bouton : 

<button class="ui teal button">Activer la facturation électronique</button>

> À noter : Une fois l'option activée, seul notre support peut faire machine arrière.

## Quid d'une institution non assujettie?

Certaines institutions, même en étant non-assujettie à la TVA, vont profiter de l'occasion pour passer à la facturation électronique, 
même si ce n'est pas obligatoire dans ce cas. Or jusqu'à présent il n'était pas possible d'introduire dans MediFleet le numéro BCE si ce 
n'était pas un numéro TVA. Nous avons modifié MediFleet et ajouté un champs dédié. Activant dès lors le reste des fonctionnalité de la 
facturation électronique pour ces institutions également.
