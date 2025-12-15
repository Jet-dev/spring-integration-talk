---
transition: fade
---

## 1️⃣ Ingestion & nettoyage des données

```mermaid
graph LR
    A[CSV utilisateurs] --> B[Lecture ligne par ligne]
    B --> C[Filtrage des emails valides]
    C --> D[Ajout d'un correlationId]
```

<v-click>

## 2️⃣ Enrichissement géographique

```mermaid
graph LR
    D[Utilisateur enrichi] --> F[Extraction pays + ville]
    F --> G[Normalisation en anglais]
    G --> H[Appel Nominatim]
    H --> I[Ville normalisée]
    H --> J[Latitude / Longitude]
```

</v-click>

<v-click>

## 3️⃣ Météo & règle métier

```mermaid
graph LR
    J[Lat / Lon] --> K[API Open météo]
    K --> L[Température & humidité]
    L --> M{> 30°C}
    M -->|Oui| N[isIceNeeded = true 🧊]
    M -->|Non| O[isIceNeeded = false]
```

</v-click>

<!--
On part d’un CSV brut, on nettoie, et on sécurise le suivi avec un correlationId.

Ici, on transforme une adresse texte en coordonnées exploitables.

C’est ici que la logique métier s’applique.
-->
