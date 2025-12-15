---
transition: fade
---

# Spring Integration en 3 points

<v-click>
<div class="flex gap-4">
<div class="w-3/4">

### 1️⃣ **C’est quoi ?**

Framework pour **implémenter les EIPs** (Enterprise Integration Patterns) en Java/Spring.
→ **Boîte à outils** pour connecter des systèmes via des _Messages_, _Canaux_ et _Endpoints_.

</div>
<div class="w-1/4 flex items-center justify-center">

<img src="https://www.enterpriseintegrationpatterns.com/img/DataEnricherIcon.gif" alt="EIP Pattern" class="w-32 h-32 object-contain" >

</div>
</div>
</v-click>
<v-click>

### 2️⃣ **Pourquoi l’utiliser ?** _(vs du code "maison")_

</v-click>

<v-click>

- **Simplicité** : Des patterns prêts à l’emploi (_Transformer_, _Router_, _Aggregator_)
- **Modularité** : Composants réutilisables (_Adapters_, _Filters_)
- **Gestion des événements** : _Polling_, _Event-Driven_, _Error Handling_

</v-click>

<v-click>

### 3️⃣ **Cas d’usage concrets** _(avec EIPs associés)_

</v-click>

<v-click>

- **Intégration de services** :
  _HTTP, Kafka, Base de données..._ (**Message Bridge**, **Channel Adapter**)
- **ETL** :
  _CSV, Transformation, API_ (**Transformer**, **Splitter**)
- **Communication entre microservices** :
  _Événements asynchrones_ (**Publish-Subscribe**, **Message Bus**)

</v-click>
