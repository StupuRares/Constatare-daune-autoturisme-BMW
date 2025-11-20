### 2.1 Sursa datelor

* **Origine:** Imagini luate de pe internet  [Descriere sursă date - ex: senzori robot, dataset public, simulare]
* **Modul de achiziție:** Antrenarea unui modul ☐ Senzori reali / ☐ Simulare / ☐ Fișier extern / ☐ Generare programatică
* **Perioada / condițiile colectării:** Noiembrie 2025 - Decembrie 2025

### 2.2 Caracteristicile dataset-ului

* **Număr total de observații:** 75
* **Număr de caracteristici (features):** 22
* **Tipuri de date:** ☐ Numerice , ☐ Imagini
* **Format fișiere:** ☐ CSV / ☐ TXT / ☐ JSON  ☐ PNG 

### 2.3 Descrierea fiecărei caracteristici

| **Caracteristică** | **Tip** | **Unitate** | **Descriere** | **Domeniu valori** |
|-------------------|---------|-------------|---------------|--------------------|
| Capotă | imagine | – | – | 3 |
| Bară față | imagine | – | – | 3 |
| Bară spate | imagine | – | – | 3 |
| Aripă față | imagine | – | – | 3 |
| Aripă spate | imagine | – | – | 3 |
| Ușă față | imagine | – | – | 3 |
| Ușă spate | imagine | – | – | 3 |
| Portbagaj / hayon | imagine | – | – | 3 |
| Parbriz | imagine | – | – | 3 |
| Lunetă | imagine | – | – | 3 |
| Geam ușă față | imagine | – | – | 3 |
| Geam ușă spate | imagine | – | – | 3 |
| Geam triunghiular spate | imagine | – | – | 3 |
| Oglindă laterală | imagine | – | – | 3 |
| Grilă față | imagine | – | – | 3 |
| Difuzor spate | imagine | – | – | 3 |
| Prag lateral | imagine | – | – | 3 |
| Far | imagine | – | – | 3 |
| Stop | imagine | – | – | 3 |
| Semnalizator lateral | imagine | – | – | 3 |
| Antenă „fin de rechin” | imagine | – | – | 3 |
| Jante (set) | imagine | – | – | 3 |


**Fișier recomandat:**  `data/README.md`

---

##  3. Analiza Exploratorie a Datelor (EDA) – Sintetic

### 3.1 Statistici descriptive aplicate

* **Distribuții pe caracteristici** (histograme)
* **Identificarea outlierilor** (IQR / percentile)

### 3.2 Analiza calității datelor

* **Detectarea valorilor lipsă** (% pe coloană)
* **Detectarea valorilor inconsistente sau eronate**
* **Identificarea caracteristicilor redundante sau puternic corelate**

### 3.3 Probleme identificate

* [exemplu] Feature X are 8% valori lipsă
* [exemplu] Distribuția feature Y este puternic neuniformă
* [exemplu] Variabilitate ridicată în clase (class imbalance)

---

##  4. Preprocesarea Datelor

### 4.1 Curățarea datelor

* **Eliminare duplicatelor**
* **Tratarea valorilor lipsă:**
  * Feature B: eliminare (30% valori lipsă)
* **Tratarea outlierilor:** IQR / limitare percentile

### 4.2 Transformarea caracteristicilor

* **Normalizare:** Min–Max / Standardizare
* **Encoding pentru variabile categoriale**
* **Ajustarea dezechilibrului de clasă** (dacă este cazul)

### 4.3 Structurarea seturilor de date

**Împărțire recomandată:**
* 70–80% – train
* 10–15% – validation
* 10–15% – test

**Principii respectate:**
* Stratificare pentru clasificare
* Fără scurgere de informație (data leakage)
* Statistici calculate DOAR pe train și aplicate pe celelalte seturi

### 4.4 Salvarea rezultatelor preprocesării

* Date preprocesate în `data/processed/`
* Seturi train/val/test în foldere dedicate
* Parametrii de preprocesare în `config/preprocessing_config.*` (opțional)

---

##  5. Fișiere Generate în Această Etapă

* `data/raw/` – date brute
* `data/processed/` – date curățate & transformate
* `data/train/`, `data/validation/`, `data/test/` – seturi finale
* `src/preprocessing/` – codul de preprocesare
* `data/README.md` – descrierea dataset-ului

---

##  6. Stare Etapă (de completat de student)

- [✔️] Structură repository configurată
- [ ] Dataset analizat (EDA realizată)
- [ ] Date preprocesate
- [ ] Seturi train/val/test generate
- [✔️] Documentație actualizată în README + `data/README.md`

---


