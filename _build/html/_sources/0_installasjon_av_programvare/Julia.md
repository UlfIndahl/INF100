---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Julia 1.10.0
  language: julia
  name: julia-1.10
---

# Installasjon av Julia på din personlige PC

Denne guiden vil hjelpe deg med å installere Julia på din PC, enten du bruker Windows eller Mac.

### Før du starter

Før du begynner installasjonen, er det viktig å vite hva slags type datamaskin du har. 


## Installasjon på Windows

1. Gå til Julia's offisielle nedlastingsside: [Julia Downloads](https://julialang.org/downloads/#current_stable_release)
2. Under "Current stable release" klikk på "Windows" og last ned <span style="color:blue;">installer</span>-filen for ditt system (__som normalt er 64-bit__). 

```{image} ../images/julia_windows_64bit.png
:alt: julia_windows64bit
:class: bg-primary mb-1
:width: 400px
:align: center
```
3. Åpne den nedlastede filen og følg instruksjonene på skjermen for å installere Julia.

<div style="display: flex; justify-content: space-between;">

```{image} ../images/julia_installason_windows_0.png
:alt: julia_windows_0
:class: bg-primary mb-1
:width: 400px
:align: left
```

```{image} ../images/julia_installasjon_windows_1.png
:alt: julia_windows_1
:class: bg-primary mb-1
:width: 400px
:align: right
```
</div>


## Installasjon på Mac 

__Hvis__ du bruker en __Mac__, må du __sjekke om__ den er basert på __Apple Silicon__ eller __Intel__.

### Hvordan sjekke om din Mac er basert på Apple Silicon eller Intel:

1. Klikk på Apple-ikonet øverst til venstre på skjermen.
2. Velg "Om denne Macen".
3. Under "Oversikt" vil du se en "Prosessor" eller "Chip"-detalj. Hvis det står "Intel", har du en Intel-basert Mac. Hvis det står "Apple M1" eller lignende, har du en Apple Silicon-basert Mac.

```{image} ../images/m1mac.png
:alt: m1mac
:class: bg-primary mb-1
:width: 400px
:align: center
```

### Installasjon på Mac (Intel)

1. Gå til Julia's offisielle nedlastingsside: [Julia Downloads](https://julialang.org/downloads/#current_stable_release)
2. Under "Current stable release" klikk på "macOS" og last ned <span style="color:blue;">.dmg</span>-filen for den __anbefalte versjonen for Intel Macs__.
3. Åpne den nedlastede .dmg-filen.
4. Dra Julia-ikonet til Applications-mappen.

### Installasjon på Mac (Apple Silicon)

1. Gå til Julia's offisielle nedlastingsside: [Julia Downloads](https://julialang.org/downloads/#current_stable_release)
2. Under "Current stable release" klikk på "macOS" og last ned <span style="color:blue;">.dmg</span>-filen for den __anbefalte versjonen for Apple Silicon Macs__.
3. Åpne den nedlastede .dmg-filen.
4. Dra Julia-ikonet til Applications-mappen.

## Etter installasjonen av Julia

Når du har installert Julia, kan du starte programmet fra startmenyen (Windows) eller Applications-mappen (Mac). Du må også følge guiden nedenfor for å installere __Visual Studio Code__ (VSC) med __Julia__ Extensionen som gjør at du enkelt kan behandle og kjøre Julia-programmer som du leser inn og/eller skriver i VSC.

Etter å ha startet Julia må du skrive inn følgende kode for å installere pakkene MAT og Plots: 

```{code-cell}
:tags: [remove-output]
using Pkg;
Pkg.add(["MAT", "Plots"])
```
**Husk å trykk enter** 

Lykke til med programmeringen i Julia!

> HUSK: Visual Studio Code guiden må også følges!
