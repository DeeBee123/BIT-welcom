---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS
css: unocss
---

# JavaScript 22.11.14

Batijos Technologijų Institutas

<!-- <div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div> -->



<style>
h1 {
  background-color: #2B90B6;
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---







# Programavimo mokykla
 
```js
while(not a programmer){
  learn
}
```



<div class="w-180 relative mt-6">
  <div class="relative w-40 h-40">
    <img
      v-motion
      :initial="{ x: 800, y: -100, scale: 1.5, rotate: -50 }"
      :enter="final"
      class="absolute top-0 left-0 right-0 bottom-0"
      src="/assets/shovel.png"
    />
  </div>

  <div
    class="text-5xl absolute top-14 left-40 text-[#2B90B6] -z-1"
    v-motion
    :initial="{ x: -80, opacity: 0}"
    :enter="{ x: 0, opacity: 1, transition: { delay: 2000, duration: 1000 } }">
    Įrankis pasiekti tikslą
  </div>
</div>

<!-- vue script setup scripts can be directly used in markdown, and will only affects current page -->
<script setup lang="ts">
const final = {
  x: 0,
  y: 0,
  rotate: 0,
  scale: 1,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
</script>


<ul>
<li> Kiek valandų realaus darbo įdedama</li>
<li> Kokia asmenybė</li>
<li> Iš kokios srities atėjote</li>
<li> Koks dabartinis žinių bagažas</li>
<li> Ar teisingai įsivaizduojame intern/junior poziciją</li>
<li> Aplikavimas į darbo pozicijas</li>
</ul>



---

# Programa

Neformali programa nuo formalios skiriasi tik tuo, kad nėra egzaminų.

<div class="grid grid-cols-3 gap-10 pt-4 -mb-6">


```mermaid {scale: 0.55}
journey
    title JavaScript programa
    section Pirmas modulis (8sav.)
      Front-end: 5: Rimantas
      Testas (Teorija + Praktika): 5
    section Antras modulis (3sav.)
      NodeJS: 5: Rimantas
      Testas (Teorija + Praktika): 5
    section Trečias modulis (10sav.)
      ReactJS: 5: Arvydas
      DB, Express: 5: Arvydas
      Mokykl. egzaminas (Teorija + Praktika): 5
```

</div>
<ul>
<li> <mdi-brain /> Testai - vyks penktadienį po modulio pabaigos.</li>
<li> <mdi-book-open-blank-variant />  Mokyklinis egzaminas - Balandžio 13d. </li>
<li> <mdi-school />  Oficialus egzaminas - Mokamas (217,83 &euro;), vyksta egzaminų centro nustatytą dieną (įprastai apie 2-3sav. po studijų)</li>
</ul>


---

# Dėstytojai
  <div  grid="~ cols-3 gap-4" border="~ gray-400 opacity-50 rounded-md" style="margin: auto">
<img src='/assets/rimas.png' alt='rimantas belovas'/>
<img src='/assets/arvydas.png' alt='arvydas kijakauskas'/>
 </div>

<img style="width: 20%; margin-top:30px" src='/assets/grupe.png' alt='simonas' />


---

# Mentoriai
  <div  grid="~ cols-3 gap-4" border="~ gray-400 opacity-50 rounded-md">
  <div >
  <img src='/assets/simona.jpg' alt='simonas' style="border-radius:50%; height: 200px; margin: auto"/>
    <h5 style="text-align: center; font-weight:bold "> Simona Zimkienė</h5>
  </div>
  <div>
 <img src='/assets/vilius.jpg' alt='vilius' style="border-radius:50%; height: 200px; margin: auto"/>
    <h5 style="text-align: center; font-weight:bold"> Vilius Ramulionis</h5>
  </div>
    <div>
  <img src='/assets/deimante.jpg' alt='deimante' style="border-radius:50%; height: 200px; margin: auto"/>
    <h5 style="text-align: center; font-weight:bold"> Deimantė Barauskaitė</h5>
  </div>
 </div>
<div  grid="~ cols-1 gap-4" border="~ gray-400 opacity-50 rounded-md" style="margin-top: 10px">
<img src='/assets/search.png' alt='simonas' />
</div>
<div  grid="~ cols-9 gap-4" style="margin-top: 5px">
<img src='/assets/call.png' alt='simonas' />
</div>
---

# Tvarkaraštis

|     |     |
| --- | --- |
| <kbd>Pirmadienis</kbd> - <kbd>Ketvirtadienis</kbd> <br/><code>12:30 - 14:55 (10min. pertrauka)</code>| Teorija |
| <kbd>Pirmadienis</kbd> - <kbd>Ketvirtadienis</kbd> <br/><code>09:35 - 12:30</code><br/><code>14:55 - 16:35</code>| <b>Praktika</b> |
| <kbd>Penktadienis</kbd>| Praktikos diena (Namų darbų atlikimas / Penktadienio iššūkiai / Testai / Penktadienio pranešimai) |
| <kbd>Nedarbo dienos</kbd> | Paskaitos nevyksta |

---

## Praktika


```mermaid {theme: 'neutral', scale: 0.8}
graph LR

B(Studentas išsiskaido uždavinį ir pradeda spręsti) -->C(Pastrigimas)
C -->|1| D[Ruby duck debugging] 
 -->|2| E[Google]
 -->|3| F[Kolegos] 
 -->|4| G[Mentorius]

```

<img style="width: 70%" src='/assets/work.png' alt='simonas' />



---

## Penktadienio pranešimai

<ul>
<li>Papildomos paskaitos (Kompiuterių architektūra, NoSQL, testavimas ir t.t.)</li>
<li>IT įmonės/ekspertai</li>
<li>HR</li>
</ul>


<img style="width: 70%" src='/assets/pp.png' alt='simonas' />



---

## Friday Challenge

Veikla penktadieniais su tikslu išmokti papildomą įrankį Figma ir nepamiršti front-end žinių.

<img style="width: 70%" src='/assets/figmaa.png' alt='simonas' />

---



## Daily Stand-ups

Robotukas kuris bus mūsų dienoraštis, padės sekti progresą ir planuoti dieną.

-  **Nuo 21d. 13:00** 
-  **Gausite žinutę iš robotuko per Teams** 
-  **Atsakyti į klausimus ką planuojame pasiekti/atlikti šiandien** 
-  **Ką pavyko pasiekti/atlikti vakar?** 
-  **Ar turite kokių blokerių?** 


<img style="width: 45%; position: relative"  src='/assets/bot.png' alt='simonas' />
<img style="width: 60%; position: absolute; bottom: -45px; right: 0"  src='/assets/dailybot.png'>

---

## Lankomumas

Aktualus su UŽT finansavimu studijuojantiems studentams. 
<ul>
<li>
Už dienas kai nedalyvaujate paskaitoje, stipendija nebus mokama.
</li>
<li>
Praktikos metu svarbu būti pasiekiamam per Teams.
</li>
</ul>

<img style="width: 70%"  src='/assets/lankom.png' alt='simonas' />


---

## Google


Įpatingai dažnai naudojamas įrankis. Patarimai efektyvesniam googlinimui:
- 🧑‍💻 **[Programavimo kalba] [raktiniai žodžiai]** - užklausos pvz. JS event bubbling, CSS variables not working, JS random number, HTML input,...
- 🧑‍💻 **Errorus dėti į kabutes** - tuomet gausime tik pagal šią frazę atsakymus
- 🧑‍💻 **site:[puslapis]** - nurodome specifinį puslapį kuriame norime rasti atsakymą. Užklausos pvz. css variables not working site:stackoverflow.com
- 🧑‍💻 **-[frazė, kuri neturėtų būti užklausoje]** - užklausos pvz. how to write components in React -class 
- 🧑‍💻 **before:[metai], after:[metai]** - užklausos pvz. React before:2019

<a href="https://www.freecodecamp.org/news/how-to-google-like-a-pro-10-tips-for-effective-googling/">Daugiau</a>

<img style="width: 70%" src="/assets/google.png" alt="google"/>

<br>


---

## Shortcuts


Laiko taupymui, greitesniam kodo rašymui:
- 🧑‍💻 **CTRL + S** - saugoti (save)
- 🧑‍💻 **CTRL + C** - kopijuoti (copy)
- 🧑‍💻 **CTRL + V** - įklijuoti (paste)
- 🧑‍💻 **CTRL + A** - pasirinkti viską (select all)
- 🧑‍💻 **CTRL + X** - iškirpti (cut)
- 🧑‍💻 **ALT + [pažymim su pelyte ką keisime]** - keisti reikšmes vienu metu keliose vietose
- 🧑‍💻 **ALT + [rodyklė į viršų] / ALT + [rodyklė žemyn]** - perkelia eilutę kodo į viršų arba į apačia
- 🧑‍💻 **CTRL + Z** - grįžti į ankstesnį pokytį (undo)\
- 🧑‍💻 **CTRL + F** - paieška faile
- 🧑‍💻 **CTRL + /** - užkomentuoja
- 🧑‍💻 **CTRL + L** - Pažymėti dabartinę eilutę
- 🧑‍💻 **CTRL + SHIFT + Z** - grįžti į vėlesnį pokytį (redo)


VScode shortcuts pdf'ai. <a href="https://vscodethemes.com/?type=dark">VS code temos</a>



---

## Kiti patarimai


- 📝 **Kalbame/skaitome/klausome kuo dažniau apie kodą** 
- 📝 **Aktyviai bendrauti grupiokais** 
- 📝 **Jei turime laisvo laiko, mokomės papildomai arba prašome papildomų užduočių** 
- 📝 **Galite susigalvoti papildomą projektą, kuriam skirtume bent po truputi laiko kasdien** 
- 📝 **Kursų eigoje tvarkomės CV, linkedin, github** 
- 📝 **Dalyvaujame programavimo renginiuose** 
- 📝 **Neperdegame ir stengiamės nepamesti savo tikslo** 




---

# SUSIPAŽINKIME 😊


<ol>
<li>Vardas?</li>
<li>Miestas?</li>
<li>Kodėl programavimas? Kodėl BIT?</li>
<li>Iš kokios srities atėjote?</li>
<li>Įdomus faktas apie tave?</li>
</ol>