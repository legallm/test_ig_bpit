<p style="padding: 5px; border-radius: 5px; border: 2px solid maroon; background: #ffffe6; width: 65%">
<b>Brief description of this Implementation Guide</b><br>
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate quis felis vel semper. In ac erat malesuada, efficitur est sit amet, hendrerit elit. Fusce mollis, dui eu sagittis vulputate, eros orci fringilla ex, in porttitor lorem nibh ut massa. Suspendisse gravida erat ante, sed faucibus libero maximus et. Aenean at est non libero aliquam porttitor.
</p>

{% if site.data.info.releaselabel == 'ci-build' %}
<div style="width: 65%">
    <blockquote class="stu-note">
    <p>Cet <i>Implementation Guide</i> n'est pas la version courante, il s'agit de la version en intégration continue soumise à des changements fréquents uniquement destinée à suivre les travaux en cours. La version courante sera accessible via l'URL canonique suite à la première release : http://interop.esante.gouv.fr/ig/test_ig_bpi</p>
    </blockquote>
</div>
{% endif %}


{% if site.data.info.releaselabel == 'public-comment' %}
<div style="width: 65%">
<blockquote class="stu-note">
<p>
  <b>Attention !</b>
  <br>
 Cet <i>Implementation Guide</i> est actuellement en concertation. La version courante est accessible à l'adresse : http://interop.esante.gouv.fr/ig/test_ig_bpi
</p>
</blockquote>
</div>
{% endif %}


<!--  A décommenter si CI-SIS  -->
<div class="figure">
    <img src="ci-sis-logo.png" alt="CI-SIS" title="Logo du CI-SIS" style="width:100%;">
</div>
<!--  -->

### Introduction

Définir ici de quoi parle l'IG (En termes non expert, compréhensible par un patient). Rajouter également les détails techniques sur le contexte et le besoin de cet IG

Les principales sections de l'IG  sont :

* Le contexte de l'IG, quelle problématique il résout
* Ce que les Implémenteurs doivent mettre en place

### Acteurs
Le tableau ci-dessous récapitule les acteurs pouvant être impliqués dans les différents processus collaboratif

{% sql {
  "query" : "
    SELECT
      Title,
      Purpose,
      Description,
      Web
    FROM Resources
    WHERE Type = 'ActorDefinition'
    ORDER BY Purpose
  ",
  "class" : "lines",
  "columns" : [
    {
      "title" : "Acteur", "type" : "link", "source" : "Title", "target" : "Web" },
    {
      "title" : "Type d'acteur", "type" : "markdown", "source" : "Purpose" },
    {
      "title" : "Description", "type" : "markdown", "source" : "Description" }
    
  ]
} %}

### Relations entre acteurs

{% include relations_acteurs.svg %}

### Dépendances

{% lang-fragment dependency-table.xhtml %}
