# Natiivi_Ohjelmointi_Tehtava3

## ✨ **Android — Calories Calculator (Jetpack Compose)**

**Tekijä:** Sara Vehviläinen  
**Oppilaitos:** Oulun ammattikorkeakoulu  
**Kurssi:** Mobiiliohjelmointi natiiviteknologioilla IN00CT07-3009  
**Lukukausi:** Kevät 2025

---

### ⭐ Tehtävän kuvaus

Tämän tehtävän tavoitteena on toteuttaa Android-sovellus, joka laskee arvioidun kalorinkulutuksen käyttäjän syöttämien tietojen perusteella: paino, sukupuoli ja fyysisen aktiivisuuden taso. Sovellus tehdään Kotliinilla ja hyödyntää Jetpack Compose -käyttöliittymäkirjastoa.

Tehtävä toimii johdantona Jetpack Composen perusrakenteisiin, kuten tilanhallintaan (`State hoisting`), käyttöliittymäkomponenttien (`OutlinedTextField`, `RadioButton`, `DropdownMenu`) luomiseen ja niiden yhdistämiseen toimivaksi kokonaisuudeksi.

---

### 🧮 Laskentakaavat

Kalorinkulutus lasketaan käyttäen seuraavia kaavoja:

*   **Mies:** `(879 + 10.2 * paino) * intensiteetti`
*   **Nainen:** `(795 + 7.18 * paino) * intensiteetti`

Intensiteettikertoimet ovat:
*   **Light:** 1.3
*   **Usual:** 1.5
*   **Moderate:** 1.7
*   **Hard:** 2.0
*   **Very hard:** 2.2
*   
---

### ✨ Toiminnallisuus

*   **Painon syöttö:** Käyttäjä syöttää painonsa `OutlinedTextField`-kenttään, joka hyväksyy vain numeroita (`KeyboardType.Number`).
*   **Sukupuolen valinta:** Käyttäjä valitsee sukupuolensa kahdesta `RadioButton`-vaihtoehdosta (Mies/Nainen).
*   **Aktiivisuustason valinta:** Käyttäjä valitsee aktiivisuustason `DropdownMenu`-pudotusvalikosta.
*   **Laskenta:** `Laske`-painike käynnistää laskutoimituksen ja päivittää tuloksen näytölle. Koko sovelluksen tilaa hallitaan keskitetysti `CalorieApp`-pääkomponentissa (`State hoisting`).
*   
---  

### 🛠️ Käytetyt teknologiat ja komponentit

*   Kotlin
*   Android Studio
*   Jetpack Compose
*   Composable-funktiot
*   State Hoisting: `remember`, `mutableStateOf`, `mutableIntStateOf`
*   Material 3 -komponentit:
    *   `OutlinedTextField`
    *   `RadioButton`
    *   `DropdownMenu`
    *   `Button`, `Column`, `Row`, `Text`, `Icon`
*   `KeyboardOptions` syötteen rajoittamiseen
  
---

### 📚 Oppimistavoitteet

*   Jetpack Composen peruskäsitteiden (Composable, Modifier) ymmärtäminen.
*   Käyttöliittymän jakaminen pienempiin, uudelleenkäytettäviin komponentteihin.
*   `State hoisting` -periaatteen soveltaminen tilanhallinnassa.
*   Erilaisten syötekomponenttien (`OutlinedTextField`, `RadioButton`, `DropdownMenu`) tehokas käyttö.
*   Sovelluksen perusrakenteen luominen ja hallinta Android Studiossa.

---

### 🌐 Oppimisresurssit

#### Jetpack Compose

*   [https://developer.android.com/jetpack/compose](https://developer.android.com/jetpack/compose) – Virallinen Compose-dokumentaatio
*   [https://developer.android.com/reference/kotlin/androidx/compose/material3/OutlinedTextField](https://developer.android.com/reference/kotlin/androidx/compose/material3/OutlinedTextField) – Tekstisyötteen käsittely
*   [https://developer.android.com/reference/kotlin/androidx/compose/material3/RadioButton](https://developer.android.com/reference/kotlin/androidx/compose/material3/RadioButton) – RadioButton-komponentti
*   [https://developer.android.com/jetpack/compose/components/dropdown-menu](https://developer.android.com/jetpack/compose/components/dropdown-menu) – Pudotusvalikot
*   [https://developer.android.com/jetpack/compose/state](https://developer.android.com/jetpack/compose/state) – Tilanhallinta (`remember`, `mutableStateOf`)

#### Android-dokumentaatio:

*   [https://developer.android.com/docs](https://developer.android.com/docs) – Virallinen Android-dokumentaatio
*   [https://developer.android.com/studio/intro](https://developer.android.com/studio/intro) – Android Studion käyttö

#### Kotlin:

*   [https://kotlinlang.org/docs/home.html](https://kotlinlang.org/docs/home.html) – Kotlin-kielen virallinen dokumentaatio

