# Projet-VisualDon

## Membres de l'équipe : William Stancu / Luka Stojanovic / Mathias Nega

## Contexte : 
Dans le cadre de ce projet, nous allons aborder le thème des sports de combat, plus précisément de l’Ultimate Fighting Championship (UFC), ainsi que l’impact qu’ils ont sur la santé cérébrale et physique des combattants, sans oublier l’aspect financier.

Les données qu’on utilise pour analyser les blessures en UFC viennent surtout des statistiques officielles de l'UFC, des commissions athlétiques (qui publient les suspensions médicales après les combats), de bases de données spécialisées en MMA et d’études scientifiques sur les commotions et traumatismes crâniens. Pour l’argent, on se base sur les bourses déclarées publiquement et sur des estimations faites par les médias, mais les vrais montants restent souvent partiellement secrets.

Le problème, c’est que ces données n’ont pas été collectées pour analyser la santé à long terme des combattants. L’UFC les collecte surtout pour le spectacle et la performance, les commissions pour respecter un cadre légal minimal, et les chercheurs pour mieux comprendre les impacts médicaux. Du coup, on mesure bien les KO, les TKO et les suspensions médicales immédiates, mais beaucoup moins les microtraumatismes répétés, le déclin cognitif progressif ou les problèmes après la carrière.

Il y a aussi un biais du côté de l’argent : les salaires publiés ne montrent pas toujours les frais d’entraînement, les commissions ou les bonus cachés. Donc, les données sont partielles et parfois orientées, ce qui peut minimiser l’impact réel des combats sur la santé physique et cérébrale, surtout pour les combattants qui gagnent peu.

## Description : 
On aura un format JSON, chaque ligne représente un combat ou un combattant, et chaque colonne correspond à un attribut précis. Par exemple, pour les combats, on a des attributs comme le nom des combattants, la date, la catégorie de poids, la durée du combat, le type de victoire (KO, TKO, soumission, décision), ainsi que les suspensions médicales éventuelles. Pour l’aspect financier, les données peuvent inclure le cash price, les bonus et parfois des estimations de revenus par sponsor. Les types de données varient : données numériques (montant en dollars, durée en secondes, nombre de KO), données catégorielles (catégorie de poids, méthode de victoire), et données textuelles (nom des combattants). Certaines données peuvent aussi être temporelles (année, date) pour analyser l’évolution des blessures ou des revenus dans le temps.

Voici un exemple :
``` json
{
  "fight_id": 1023,
  "event": "UFC 280",
  "date": "2022-10-22",
  "fighter_1": "Charles Oliveira",
  "fighter_2": "Islam Makhachev",
  "weight_category": "Lightweight",
  "rounds": 2,
  "duration_seconds": 189,
  "method": "Submission",
  "ko": false,
  "medical_suspension_days_fighter_1": 0,
  "medical_suspension_days_fighter_2": 30,
  "purse_fighter_1": 750000,
  "purse_fighter_2": 500000,
  "bonus_fighter_1": 0,
  "bonus_fighter_2": 0,
  "estimated_sponsor_revenue_fighter_1": 50000,
  "estimated_sponsor_revenue_fighter_2": 40000
}
```
## But : 
On veut autant explorer qu’expliquer dans notre cas.

Explorer, parce qu’on veut regarder les tendances dans les données : combien de KO il y a, si les blessures augmentent avec le temps, si les combattants qui font beaucoup de combats ont plus de suspensions médicales, ou encore s’il y a un lien entre le nombre de combats et les revenus. Mais on veut aussi expliquer quelque chose de plus précis, en guidant le lecteur vers une réflexion plus large.

L’histoire qu’on veut raconter, c’est un peu la face cachée de l’UFC. Derrière le show, les gros événements et les highlights spectaculaires, il y a des combattants qui accumulent des blessures physiques et cérébrales. Certains encaissent des KO répétés et prennent des risques énormes pour leur santé, alors que leurs revenus ne sont pas toujours à la hauteur, surtout pour ceux qui ne sont pas des grandes stars.

On ne veut pas critiquer, mais plutôt apporter de la lumière sur des faits malheureux derrière cette organisation.

## Références :
On utilisera des sites web de l'UFC pour l'historique des combats de chaque combattant ainsi que d'autres site indicatif pour les blessures et salaires.

https://statleaders.ufc.com/ <br>
https://www.rotowire.com/mma/injury-report.php <br>
http://ufcstats.com/ <br>
https://combatsmma.fr/combien-gagnent-les-combattants-ufc-par-combat-les-vrais-chiffres-reveles <br>

