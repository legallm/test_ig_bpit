<p style="padding: 5px; border-radius: 5px; border: 2px solid maroon; background: #ffffe6; width: 65%">
<b>Brief description of this Implementation Guide</b><br>
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate quis felis vel semper. In ac erat malesuada, efficitur est sit amet, hendrerit elit. Fusce mollis, dui eu sagittis vulputate, eros orci fringilla ex, in porttitor lorem nibh ut massa. Suspendisse gravida erat ante, sed faucibus libero maximus et. Aenean at est non libero aliquam porttitor.
</p>

{% if site.data.info.releaselabel == 'ci-build' %}
<div style="width: 65%">
    <blockquote class="stu-note">
    <p>Cet Implementation Guide n'est pas la version courante, il s'agit de la version en intégration continue soumise à des changements fréquents uniquement destinée à suivre les travaux en cours. La version courante sera accessible via l'URL canonique suite à la première release : http://interop.esante.gouv.fr/ig/test_ig_bpi</p>
    </blockquote>
</div>
{% endif %}


{% if site.data.info.releaselabel == 'public-comment' %}
<div style="width: 65%">
<blockquote class="stu-note">
<p>
  <b>Attention !</b>
  <br>
 Cet Implementation Guide est actuellement en concertation. La version courante est accessible à l'adresse : http://interop.esante.gouv.fr/ig/test_ig_bpi
</p>
</blockquote>
</div>
{% endif %}


<!--  A décommenter si CI-SIS
<div class="figure">
    <img src="ci-sis-logo.png" alt="CI-SIS" title="Logo du CI-SIS" style="width:100%;">
</div>
-->

### Introduction

Définir ici de quoi parle l'IG (En termes non expert, compréhensible par un patient). Rajouter également les détails techniques sur le contexte et le besoin de cet IG

Les principales sections de l'IG  sont :

* Le contexte de l'IG, quelle problématique il résout
* Ce que les Implémenteurs doivent mettre en place
* Un onglet "Ressources de conformité" pour s'assurer d'un schéma global entre tous les IGs

### Glossaire 
- **Toto** : Lorem ipsum dolor sit amet, consectetur. 
- **Tutu** : Lorem ipsum dolor sit amet, consectetur adipiscing elit.

### Auteurs et contributeurs (optionnel)

| Role               | Nom        | Organisation                 | Contact                  |
| ------------------ | ---------- | ---------------------------- | ------------------------ |
| **Primary Editor** | Prenom Nom | Agence du Numérique en Santé | prenom.nom@address.email |

### Dépendances

{% include dependency-table.xhtml %}

### Propriété intellectuelle

{% include ip-statements.xhtml %}
