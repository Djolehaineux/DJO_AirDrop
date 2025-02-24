# DJO_AirDrop
Bienvenue sur Mon guide d'installation est de configuration pour mon mods DJO_AirDrop

### Déscriptions
Ce mod est mon premier mod d'AirDrop, il peut être entièrement configurable.  
Vous pouvez aussi bien l'utiliser avec mes containers que avec des containers provenant d'autres mods.  
Les AirDrop générés n'ont pas de persistance et sont donc supprimés de la carte à chaque redémarrage.  
Un message est envoyé a tous les joueurs dans le canal de chat à chaque génération d'Airdrop.  
Le fait de pouvoir paramétrer le type de caisse et les créatures offre la possibilité de l'utiliser pour créer des hordes.


## INSTALLATION
- Placer le mod à la racine de votre serveur. (dans le dossier 📂**dayzstandalone**)
- Placer la key qui se trouve à l'intérieur du dossier 📂**KEY** du mod dans le dossier 📂**KEY** de votre serveur.
- Ajoutez `@DJO_AirDrop` a la barre de lancement de vot mods.  
(la configurations peux changer suivant l'hebergeur)
- Un dossier `DJO_AirDrop`contenant un fichier `Settings.json` serat crée dans le dossier `profile / config` de votre serveur des le premier démarage.

### Guide Configurations de La gestion d'apparitions des **AirDrop**
```
{
    "ConfigVersion": "1",
    "isEnabled": 1,
    "spawnInterval": 1800.0,
    "cleanTime": 1200.0,
    "isFullyInitialized": 0,
    "airdropTypes": [
        "AirDrop_T1"
        // ici vous pouvez ajoutez de nouveaux container exemple: SeaChest
    ],
    "airdropTypeConfigs": {
        "AirDrop_T1": {
            "positions": [
                {
                    "position": [
                        11872.8017578125,
                        140.00003051757813,
                        12555.943359375
                    ],
                    "message": "Alerte! Un airdrop a atterri a l' Airfield! (Krasno)"
                }
                // ici vous pouvez ajoutez de nouvel position
            ],
            "spawnCountMin": 1,
            "spawnCountMax": 1,
            "airdropLoot": {
                "categories": {
                    "Weapons_01": 1
                    // ici vous pouvez ajoutez de nouvel categories d'items
                }
            },
            "creatureCountMin": 5,
            "creatureCountMax": 10,
            "creatureTypes": [
                "ZmbF_PoliceWomanNormal",
                "Animal_CanisLupus_Grey"
                // ici vous pouvez ajoutez de nouvel créature
            ]
        }
        // ici vous pouvez ajoutez les nouveaux container
    },
```
`"isEnabled": 1,` Activer ou désactiver les AirDrop (1 = Activer / 0 = Désactiver).  
`"spawnInterval": 1800.0,`Intervalle entre chaque vague d'apparition des AirDrop (Temps défini en seconde = 30 minutes).  
`"cleanTime": 1200.0,`Temps avant suppression des AirDrop dans le monde (Temps défini en seconde = 20 minutes).  
`"airdropTypeConfigs"` Gestion des apparitions des différents types d'AirDrop.  
`"AirDrop_T1"` Début de la configuration de l'AirDrop_T1.  
`"positions"` Class qui définit l'ensemble des positions pour l'AirDrop_T1.  
`"position"` Points d'apparition des AirDrop, valeur des pos `X`, `Y`, `Z`  
`"message"` Contenu du message qui sera envoyé en jeu lors de l'apparition.  
`"spawnCountMin": 1,` Quantité minimum d'AirDrop_T1 peuvent être générées en même temps.  
`"spawnCountMax": 2,` Quantité maximum d'AirDrop_T1 peuvent être générées en même temps.  
`"airdropLoot"` Class contenant la gestion d'apparitions du loot.  
`"categories"` Class d'appel aux différentes catégories d'items.  
`"WeaponsT1": 1,` Nom de la catégorie appelée pour générer le butin à l'intérieur de l'AirDrop et la quantité de pack d'items demandée  
`"creatureCountMin": 5,` Quantité minimum de créatures rattachées à l'airdrop.  
`"creatureCountMax": 10,` Quantité maximale de créatures rattachées à l'airdrop.  
`"creatureTypes"` Class contenant les différents types de créatures. Vous pouvez aussi bien placer des zombies que des animaux.  
`"ZmbF_PoliceWomanNormal"` Nom types d'un zombie.  
`"Animal_CanisLupus_Grey"` Nom types d'un loup.  

### Guide Configurations de La gestion du loot des **AirDrop**
```
    "Categories": {
		"WeaponsT1": [
			"Pack1": {
				{
					"item": "M4A1",
					"attachments": [
						"M4_CQBBttstck",
						"M4_MPHndgrd",
						"ACOGOptic_6x",
						"M4_Suppressor",
						"Mag_STANAG_60Rnd"
					]
				},
				{
					"item": "Mag_STANAG_60Rnd",
					"attachments": []
				},
				{
					"item": "Ammo_556x45",
					"attachments": []
				}
			},
			"Pack2": {,
				{
					"item": "Aug",
					"attachments": [
						"ACOGOptic_6x",
						"M4_Suppressor",
						"Mag_STANAG_60Rnd"
					]
				},
				{
					"item": "Mag_STANAG_60Rnd",
					"attachments": []
				},
				{
					"item": "Ammo_556x45",
					"attachments": []
				}
			}
		],
        // Ici vous pouvez rajoutez de nouvel Categories
    }
}
```
`"Categories"` Class contenant les différentes catégories d'items.  
`"WeaponsT1"` Nom de la catégorie.   
`"Pack1"` Nom du Pack d'items a invoquer.   
`"Pack2"` Nom du Pack d'items a invoquer.  
`"item": "M4A1"` Déclarations d'un item `M4A1`, noms types de l'items.   
`"attachments"`  Déclarations des attachements de l'items.  
`"M4_CQBBttstck"` Nom types de l'attachement.  


[exemple](https://github.com/Djolehaineux/DJO_AirDrop/blob/main/Exemple_Settings.json) d'intégration d'un nouveau conteneur avec une nouvelle catégorie d'items.  

Si vous avez encore besoin d'aide, n'hésitez pas à rejoindre mon [DISCORD](https://discord.gg/UXNKcxApkU) pour obtenir de l'aide.

---

[retourner a la collections](https://github.com/Djolehaineux/DJO-mods-collection)
