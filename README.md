# Gestion Comptable & RH — HCR / BTP

Application web **100 % locale** : gestion comptable et RH **multi-sociétés** (convention HCR & promoteur/BTP) et **multi-années**, qui fonctionne directement dans le navigateur d'un PC d'entreprise **sans installation, sans exécutable, sans connexion internet**.

## 🚀 Ouvrir l'application (aucun droit requis)

1. Copiez le dossier (ou au minimum le fichier **`index.html`**) sur le PC (ex. dans `Documents`).
2. **Double-cliquez sur `index.html`** → il s'ouvre dans votre navigateur (Chrome, Edge ou Firefox).
3. C'est tout. Aucun `.exe`, aucun `.bat`, aucune installation, aucun droit administrateur.

> 💡 **Astuce pour l'ouvrir en 1 clic** : clic droit sur `index.html` → « Épingler au menu Démarrer » ou créer un raccourci sur le Bureau.
>
> ℹ️ Les données sont stockées dans le **profil du navigateur** (localStorage). Utilisez toujours le **même navigateur et le même profil** (évitez le mode navigation privée, qui efface le stockage à la fermeture).

## 💾 Sauvegardes

- **Automatique** : chaque saisie est enregistrée instantanément dans le navigateur (compteur « 💾 » en haut à droite).
- **Exporter sauvegarde (.json)** : bouton toujours visible en haut. Faites-le **régulièrement** (ex. fin de saison et fin d'année) : c'est votre archive pérenne et votre filet de sécurité (changement de PC, panne, nettoyage du navigateur).
- **Importer sauvegarde (.json)** : restaure l'intégralité des données (toutes sociétés, toutes années).
- **Exporter CSV / Excel** : disponible sur chaque tableau clé (budget, factures, situation, semaines, décompte, chantiers). Ouvre directement dans Excel.

## 🗂️ Utilisation

| Onglet | Contenu |
|---|---|
| 🏠 **Tableau de bord** | Synthèse société/année : totaux, coûts mensuels, top catégories, synthèse chantiers. |
| 🧾 **Factures & Budget** | Saisie rapide de facture (dates, **mois de réalisation AAAA-MM**, fournisseur, HT/TTC, catégorie, chantier). Tableau **Catégories × Mois de réalisation** avec totaux mensuels, cumul annuel et filtres. |
| 🏨 **Situation Hôtel** (HCR) | Encaissements mensuels par **mode de règlement** (grille éditable, personnalisable), totaux mensuels et annuels. |
| 👥 **RH HCR & Heures supp** | Employés (39 h/35 h, saison, taux horaire) · **Pointage** arrivée/départ/pause par jour · calcul **hebdomadaire** des heures supp (+10 %, +20 %, +50 %) · **Fiches de paie** (heures payées + coût global employeur, intégré au budget) · **Décompte fin de saison** par taux : heures dues − payées = solde, en heures et en €. |
| 🏗️ **Chantiers BTP** | Coût global par employé/mois, **demi-journées par chantier**, factures rattachées, **synthèse par chantier** avec main-d'œuvre **proratisée** (coût × DJ chantier ÷ DJ totales). |
| ⚙️ **Paramètres & Sauvegarde** | Sociétés (créer/renommer/désactiver), années, catégories, modes de règlement, **seuils et taux des heures supp éditables**, employés, exports/imports. |

### Logique des heures supplémentaires ( Hebdomadaire, conforme à l'exemple )
Les heures sont totalisées **par semaine calendaire (norme ISO)** puis ventilées selon les tranches paramétrées
(défaut : 35–39 h → +10 %, 39–43 h → +20 %, au-delà de 43 h → +50 %).
Exemple vérifié : contrat 39 h lissé (151,67 h + 17,33 h à +10 % par mois) — une semaine à **35 h** puis une semaine à **43 h**
⇒ **70 h normales, 4 h à +10 %, 4 h à +20 %** (et non un calcul lissé qui masquerait ces heures).
Le décompte de fin de saison compare par taux les heures **dues** (calcul hebdomadaire cumulé) et les heures **payées** (fiches de paie ; si le détail +10/+20/+50 n'est pas saisi, il est estimé par lissage et indiqué « ≈ estimé »).

## 📁 Contenu

- `index.html` — l'application complète (HTML + CSS + JavaScript dans un seul fichier autonome).
- `README.md` — cette notice.

## 🔒 Confidentialité

Aucune donnée ne quitte le PC : pas de serveur, pas de site internet, pas de compte. Le fichier fonctionne hors ligne.
