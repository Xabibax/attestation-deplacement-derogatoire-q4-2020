# Mon générateur de certificat de déplacement

## Prérequis

* [Node.js / npm](https://nodejs.org/en/) 

## Utilisation

### Installer le projet

```console
git clone https://github.com/Xabibax/attestation-deplacement-derogatoire-q4-2020.git
cd attestation-deplacement-derogatoire-q4-2020
npm i
```

### Personaliser la génération de l'attestation

Le fichier profile.js (src/js/profile.js) sert à générer automatiquement le profile de l'attestation.  
La date et l'heure de sortie de l'attestation sont récupérées à partir de celles du formulaire, qui sont elles-mêmes en fonction de la date et l'heure de consultation de la page (F5 pour mettre à jour).

### Générer l'attestation

Lancez l'application :

```console
npm start
```

Rendez-vous à l'url indiqué (ex: http://localhost:1234) :

```console
Server running at http://localhost:1234 
```

Adaptez la date et l'heure de sortie à votre convenance (ne modifie la date et l'heure de création du QR code).  
Sélectionnez votre motif de sortie.  
Cliquez sur le bouton "Mon attestation personalisée" pour générer l'attestation avec votre profil.  

Le bouton standard reste disponible pour une utilisation standard de l'application.

## Crédits

Ce projet a été réalisé à partir d'un fork du dépôt [attestation-deplacement-derogatoire-q4-2020](https://github.com/LAB-MI/attestation-deplacement-derogatoire-q4-2020) lui-même réalisé à partir d'un fork du dépôt [deplacement-covid-19](https://github.com/nesk/deplacement-covid-19) lui-même réalisé à partir d'un fork du dépôt [covid-19-certificate](https://github.com/nesk/covid-19-certificate) de [Johann Pardanaud](https://github.com/nesk).

Les projets open source suivants ont été utilisés pour le développement de ce
service :

- [PDF-LIB](https://pdf-lib.js.org/)
- [qrcode](https://github.com/soldair/node-qrcode)
- [Bootstrap](https://getbootstrap.com/)
- [Font Awesome](https://fontawesome.com/license)
