---
transition: fade
---

# Pourquoi parler d’intégration ?

## Le constat

<div v-motion
     :initial="{ opacity: 0, y: 20 }"
     :enter="{ opacity: 1, y: 0, transition: { delay: 200 } }">

**Problématique** :
_"On a des données <span v-mark.circle.red>partout</span>… mais elles ne se parlent pas !"_
→ CSV, Kafka, APIs, bases de données, SaaS… **comment tout faire communiquer ?**

<v-click>

**Enjeux clés** :
</v-click>
<v-click>

- Connecter des systèmes ✅

</v-click>

<v-click>

- Automatiser les processus ⚡

</v-click>

<v-click>

- Éviter la <span v-mark.underline.red="5">saisie manuelle</span> (et les erreurs !)

</v-click>

</div>

<v-click>

## Mon parcours

</v-click>

<div v-motion
     :initial="{ x: -100, opacity: 0 }"
     :enter="{ x: 0, opacity: 1 }">

<v-click>

- **Déclic** : Projet <span v-mark.circle.blue="7">Learning & Development</span> chez Decathlon

</v-click>
<v-click>

- **Mission** :
  Intégrer des données collaborateurs (utilisateurs, compétences, postes) dans des **SaaS externes**

</v-click>

</div>

<div v-motion
     :initial="{ x: -100, opacity: 0 }"
     :enter="{ x: 0, opacity: 1 }"
     :delay="200">

<v-click>

> _"Et si on pouvait synchroniser tout ça… sans y passer des semaines de dev ?"_

</v-click>

</div>
