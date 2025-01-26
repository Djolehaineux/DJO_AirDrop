# DJO_AirDrop
Bienvenue sur Mon guide d'installation est de configuration pour mon mods DJO_AirDrop



## INSTALLATION
- Placer le mod a la racine de votre serveur
- Placer la key qui se trouve à l'intérieur du dossier KEY du mod dans le dossier key de votre serveur
- Déclarée le mods dans la barre de lancement de votre serveur


### FICHIER FOURNI
- 

### Guide Configurations
Activer ou désactiver les AirDrop `"isEnabled": 1,` 1 = Activer / 0 = Désactiver
Interval entre chaque vague d'apparition des AirDrop `"spawnInterval": 1800.0,` Temps definie en seconde (30 minutes)
Temps avant suppression des AirDrop dans le monde `"cleanTime": 1200.0,` Temps definie en seconde (20 minutes)

Nom types des diférent AirDrop
```
"airdropTypes": [
    "AirDrop_T1",
    "AirDrop_T2",
    "AirDrop_T3",
    "AirDrop_T4"
],
```
Gestion des apparition des AirDrop `"airdropTypeConfigs"` 
<p>`AirDrop_T1` Début de la configuration de l'AirDrop_T1<p/>

<p>`"positions"` class qui definie l'enssemble des position pour l'AirDrop_T1 <p/>
<p>`"position"` points d'apparitions des AirDrop valeur des pos `X`, `Y`, `Z` <p/>
<p>`"message"` contenue du message qui sera envoyée en jeux lors de l'apparitions <p/>
**EXEMPLE:**
```
{
    "position": [
        11872.8017578125,
        140.00003051757813,
        12555.943359375
    ],
    "message": "Alerte! Un airdrop a atterri a l' Airfield! (Krasno)"
}
```
---

[retourner a la collections](https://github.com/Djolehaineux/DJO-mods-collection)
