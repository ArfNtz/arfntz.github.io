Créer un programme en respectant cette Spécification Fonctionnelle.

## Titre : BAM 2025/2026, Calculateur inscription famille

---

### 🎯 Objectif

Permettre aux familles d'estimer leur **montant d'inscription annuel** à La Boîte à Musique (BAM), selon :

* les types de cours choisis (individuels ou collectifs)
* le quotient familial CAF
* le statut de résident (Savenay)
* l’âge de l’élève (< 18 ans ou étudiant)
* les règles de réduction BAM
* les arrondis et cotisation familiale

---

## 1. 🧾 Entrées utilisateur

| Intitulé                         | Type                     | Valeurs possibles                                      |
| ------------------------------ | ------------------------ | ------------------------------------------------------ |
| **Quotient familial (QF)**     | Liste                  | `>1500`, `1350`, `1050`, `900`, `750`, `0`             |
| **Résident Savenay**           | Case            | Oui / Non                                              |
| **Moins de 18 ans / étudiant** | Case          | Oui / Non                                              |
| **Instrument 1ère année (binôme)**        | Bouton            | 1,2,3                                     |
| **Instrument 2e année et + (individuel)** | Bouton            | 1,2,3                                     |

---

## 2. 💸 Tarifs

### 🎼 **Cours individuels**

**Non résident Savenay**

| Type de cours                         | Plus de 18 ans               | Moins de 18 ans      | 
| ------------------------------------- | ---------------------------- | -------------------- |
| Instrument 1ère année (binôme)        |                              | 525 €                |
| Instrument 2e année et + (individuel) | 843 €                        | 759 €                |

**Résident Savenay**

| Type de cours                         | Plus de 18 ans               | Moins de 18 ans      | 
| ------------------------------------- | ---------------------------- | -------------------- |
| Instrument 1ère année (binôme)        |                              | 384 €                |
| Instrument 2e année et + (individuel) | 762 €                        | 543 €                |

### 🎤 **Cours collectifs (ateliers)**

| Atelier                  | Tarif (fixe) |
| ------------------------ | ------------ |
| Atelier éveil            | 102 €        |
| Atelier chant            | 126 €        |
| Chorale adulte           | 156 €        |
| Atelier orchestre jeunes | 156 €        |
| Atelier orchestre adulte | 186 €        |
| Formation musicale       | 126 €        |

---

## 3. 📉 Réductions

### 🎼 Sur les **cours individuels uniquement**

#### 📊 Réduction selon quotient familial (QF)

| QF CAF        | Réduction si < 18 ans | Réduction si ≥ 18 ans |
| ------------- | --------------------- | --------------------- |
| > 1500 €      | 0%                    | 0%                    |
| 1350 – 1500 € | 5%                    | 0%                    |
| 1050 – 1350 € | 10%                   | 0%                    |
| 900 – 1050 €  | 15%                   | 0%                    |
| 750 – 900 €   | 30%                   | 0%                    |
| 0 – 750 €     | 80%                   | 80%                   |

#### 👨‍👩‍👧 Réduction **famille**

* Si **≥ 2 cours individuels** cochés dans une même simulation
* ➡ **-5%** supplémentaires sur le total des cours individuels (après réduction QF)

---

### ❌ **Aucune réduction sur les cours collectifs**

* Tarifs fixes
* Aucune réduction liée au QF, Savenay ou âge

---

## 4. 🎁 Règle de gratuité sur les ateliers

| Situation                                      | Gratuité appliquée                          |
| ---------------------------------------------- | ------------------------------------------- |
| ≥1 cours individuel sélectionné                | 1 atelier collectif gratuit (le moins cher) |
| ≥2 ateliers collectifs, aucun cours individuel | 1 atelier gratuit (le moins cher)           |
| 1 seul atelier collectif, aucun cours ind.     | Aucun gratuit                               |

* ✅ **Maximum 1 atelier gratuit par inscription**
* ✅ Si plusieurs ateliers sont cochés, **le moins cher devient gratuit**

---

## 5. 💶 Cotisation annuelle

* **+40 € par famille** (obligatoire)

---

## 6. 📋 Affichage

Afficher l'objectif en haut de page.
Afficher les détails des calculs.
Afficher le tableau des tarifs selon les conditions en bas de page.
Afficher les règles de réduction.


---

## 7. 📱 Accessibilité & compatibilité

* Interface légère, responsive et utilisable sur :

  * ✅ **iPhone/iPad (Safari iOS)**
  * ✅ **Android (Chrome)**
  * ✅ **Navigateurs desktop (Chrome, Firefox, Edge…)**
* Aucun enregistrement ni cookie requis

