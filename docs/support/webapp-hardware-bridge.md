# 🖥️ WebApp Hardware Bridge

> **Installation et Configuration (Windows)**  

---

## 📘 Description

**WebApp Hardware Bridge (WHB)** est une application permettant de relier l’ERP **LÉO** à vos **imprimantes locales**.  
Une fois configurée, elle permet d’imprimer vos documents directement depuis LÉO en **un seul clic**.

---

## ⚙️ Installation

### 🔽 1. Téléchargement

1. Accédez à la page officielle du projet :  
   👉 [https://github.com/imTigger/webapp-hardware-bridge/releases](https://github.com/imTigger/webapp-hardware-bridge/releases)
2. Dans la section **Assets**, téléchargez le fichier suivant :  
   **`whb-1.0.0.exe`**

---

### 🧭 2. Étapes d’installation

1. Double-cliquez sur le fichier téléchargé (**whb-1.0.0.exe**) dans le dossier *Téléchargements*.
2. Suivez l’assistant d’installation standard de Windows.
3. Cochez l’option **Auto-start** pour permettre le démarrage automatique à chaque ouverture de session.
4. Une fois installé, **l’application s’exécute en arrière-plan** et son icône s’affiche dans la **zone de notification Windows** (près de l’horloge système).

> 💡 **Astuce :**  
> Si WHB est déjà lancé, faites un **clic droit** sur son icône et choisissez **Web UI** pour ouvrir la fenêtre de configuration dans votre navigateur.

---

## 🖨️ Configuration

### 🧾 1. Ajouter une imprimante

1. Depuis la **zone de notification**, clic droit sur **l’icône WHB** → **Web UI**.  
2. Dans l’onglet **Printers**, cliquez sur **+** pour ajouter une nouvelle imprimante.  
   Un onglet *Printer 1* s’ouvre automatiquement.
3. Dans la colonne **Type**, saisir : `MAIN`.  
4. Dans la colonne **Print Name**, sélectionnez l’imprimante souhaitée (ex. : *HP LaserJet 4100*).

---

### 🌐 2. Paramétrer le serveur

Dans l’onglet **Web / WebSocket Server**, remplissez les champs suivants :

| Champ | Valeur |
|-------|--------|
| **Bind** | `127.0.0.1` |
| **Address** | `127.0.0.1` |
| **Port** | `12212` |

> ⚠️ **Attention :**  
> Ces valeurs doivent impérativement être respectées pour assurer la communication entre **LÉO** et **WHB**.

Cliquez sur **Save** pour enregistrer les réglages.

---

## 🚀 Utilisation

Une fois WHB configuré :

- L’imprimante est reliée à LÉO.
- L’impression de documents (devis, bons de livraison, factures, etc.) se fait **en un clic**, directement depuis l’ERP.

> 🖨️ **Astuce :**  
> En cas de changement d’imprimante, il suffit de répéter les étapes de configuration.

---

## 🧰 Dépannage

| Problème | Cause possible | Solution |
|-----------|----------------|-----------|
| L’imprimante ne répond pas | Port bloqué ou adresse erronée | Vérifiez le port **12212** et les adresses **127.0.0.1** |
| L’application ne démarre pas | Option *Auto-start* non activée | Ouvrez WHB manuellement depuis le menu Démarrer |
| Impression lente | Mauvais pilote ou réseau saturé | Mettez à jour le pilote de l’imprimante |

---

## ✅ Conclusion

Votre poste est désormais connecté à votre imprimante via **WebApp Hardware Bridge**.  
Vous pouvez désormais imprimer directement depuis **LÉO**, sans passer par les fenêtres d’impression Windows.

---

## 📎 Informations complémentaires

- **Projet GitHub** : [imTigger/webapp-hardware-bridge](https://github.com/imTigger/webapp-hardware-bridge)  
- **Auteur** : *Alex Lamizana — Service Informatique, Landreau Groupe*  
