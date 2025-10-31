Sehr geehrte Damen und Herren, geschätzte Kollegen,

als Masterstudent der Angewandten Physik freue ich mich, Ihnen heute in den nächsten 10 Minuten einen prägnanten Überblick über die **Wechselwirkungen geladener Teilchen mit Materie** zu geben, ein fundamentales Feld, dessen theoretische Grundlagen die Basis für moderne Anwendungen von der Dosimetrie bis zur Hadronentherapie bilden.

---
[TOC]
### Gliederung des Vortrags

1. **Einleitung: Aktuelle Relevanz und Aufhänger (Attention Catcher)**
2. **Das Bremsvermögen (Stopping Power): Mechanismen und Definitionen**
3. **Die Bethe-Formel und die Dynamik des Kollisionsverlusts**
4. **Die Form der Bethe Mass Collision Stopping Power Curve**
5. **Makroskopische Konsequenzen: Der Bragg-Peak**
6. **Zusammenfassung**

---

### 1. Einleitung: Aktuelle Relevanz

Die präzise Steuerung und Dosierung geladener Teilchen ist ein Eckpfeiler der modernen Medizinphysik. Im Kontext der **Hadronentherapie**—insbesondere der Protonen- oder Schwerionentherapie—entscheidet die genaue Vorhersage des Energieverlusts darüber, ob der Bragg-Peak millimetergenau im Tumorgewebe platziert wird, während umliegendes gesundes Gewebe geschont bleibt.

Dieser kritische Bereich der Dosimetrie baut direkt auf den theoretischen Modellen auf, die erklären, wie geladene Teilchen ihre kinetische Energie schrittweise in einem absorbierenden Medium abgeben. Das Verständnis des **Bremsvermögens** ist daher nicht nur ein historisches Thema, das mit Bohr (1913) begann und mit Bethe und Fano (1930er/1960er) kulminierte, sondern es ist eine aktive Notwendigkeit für die klinische Präzision.

``Bild: Titlepage ``

---

### 2. Das Bremsvermögen (Stopping Power)

Ein geladenes Teilchen, das in Materie eindringt, ist von seinem Coulomb-Feld umgeben, welches sowohl mit den Orbitalelektronen als auch mit den Atomkernen des Absorbers wechselwirkt. Die resultierenden Energieüberträge bestimmen, wie schnell das Teilchen seine kinetische Energie verliert – genau diese Verlustleistung fasst das Bremsvermögen.

#### Definitionen und Zusammensetzung

Das **lineare Bremsvermögen** beschreibt den Energieverlust pro Einheitsweg $(−dE/dx)$ in MeV/cm. Teilt man diesen Ausdruck durch die Dichte $\rho$ des Absorbers, erhält man das **Massenbremsvermögen**
$$ S = -\frac{1}{\rho} \frac{dE}{dx} $$
mit der Einheit $\text{MeV} \cdot \text{cm}^2 \cdot \text{g}^{-1}$.

Das **Gesamt-Massenbremsvermögen** setzt sich additiv aus Kollisions- und Strahlungsanteil zusammen:
$$ S_{tot} = S_{col} + S_{rad} \; . $$

#### Strahlungsverlust (S_rad, Bremsstrahlung)

Der Strahlungsverlust beschreibt die Energieabgabe durch Bremsstrahlung infolge der Wechselwirkung mit den Atomkernen des Absorbers.

`` Bild: CollisionTypes ``

Bei **sehr kleinem Stoßparameter gegenüber dem Atomradius ($b \ll a$)** wird das Projektil vom Atomkern stark abgelenkt und emittiert Bremsstrahlung.
Die mittlere Verlustleistung wächst mit der kinetischen Energie, skaliert nahezu quadratisch mit der Kernladungszahl des Absorbers ($\propto Z^2$) und fällt mit dem Quadrat der Teilchenmasse ($\propto 1/m^2$). Für Elektronen/Positronen kann der Strahlungsanteil daher den Kollisionsanteil übersteigen; für Protonen und schwerere Ionen bleibt er vernachlässigbar.
Der Übergangspunkt, an dem Strahlung und Kollision gleich wichtig werden, ist die **kritische Energie** $E_{K,crit}$

#### Kollisionsverlust (S_col)

Der Kollisionsverlust beschreibt die mittlere Energieabgabe an Orbitalelektronen und führt zu Anregung oder Ionisation (Electronic Stopping Power). Für schwere Projektile ist dies der dominante Term, da der Strahlungsanteil unterdrückt ist. In der Praxis wird der Kollisionsverlust in weiche und harte Beiträge zerlegt:
$$ S_{col} = S_{soft}^{col} + S_{hard}^{col} \; . $$

#### Mikroskopische Komponenten des Kollisionsverlusts

Die mikroskopischen Wechselwirkungen werden klassisch über den Stoßparameter $b$ relativ zum Atomradius $a$ charakterisiert:

`` nochmal: Bild: CollisionTypes ``

1. **Weiche (distant) Kollisionen ($b \gg a$):** Das Teilchen spürt das gesamte Atom, der Energieübertrag pro Ereignis ist klein, die Häufigkeit jedoch groß. Diese Prozesse führen zu Polarisation, Anregung und Ionisation und tragen rund die Hälfte zu $S_{col}$ bei.
2. **Harte (close) Kollisionen ($b \approx a$):** Direktes Coulomb-Wechselwirkung an einzelnen Elektronen verursacht große Energieüberträge. Die ausgelösten $\delta$-Elektronen sind selbst ionisierend und liefern den restlichen Beitrag zu $S_{col}$.

---

### 3. Die Bethe-Formel und die Dynamik des Kollisionsverlusts

Für schwere geladene Teilchen ist die **Kollisionsbremskraft** ($S_{col}$) der dominierende Term. Die historische Entwicklung führte von Bohrs klassischer Theorie (1913), die die Bindungseffekte nur rudimentär berücksichtigte und experimentelle Daten um einen Faktor 2 unterschätzte, zu Bethes quantenmechanisch-relativistischer Theorie (1931).

#### Herleitungskontext der Bethe-Formel
 
Bethe unterteilte $S_{col}$ in $S_{soft}$ und $S_{hard}$. Bei der Zusammenfassung der Terme (Gleichung 6.40 und 6.41) fällt die willkürlich gewählte Energieabgrenzung $\eta$ zwischen weichen und harten Kollisionen heraus.

Das Ergebnis für schwere geladene Teilchen (Bethe Mass Collision Stopping Power Equation) lautet (ohne Korrekturen):

$$ S_{col} = C_0 \frac{z^2}{A\beta^2} Z \left\{ \ln \frac{2m_e c^2}{I} + \ln \frac{\beta^2}{1-\beta^2} - \beta^2 \right\} $$

#### Erklärung der Terme und Aspekte

1. **Teilchenladung und Geschwindigkeitsterm $\left( C_0 \frac{z^2}{A\beta^2} Z \right)$:**
    * $z^2$: Die Bremskraft ist proportional zum Quadrat der Ladung des Projektils ($z$).
    * $1/\beta^2$: Im nicht-relativistischen und intermediären Bereich ist die Bremskraft umgekehrt proportional zum Quadrat der Teilchengeschwindigkeit ($\beta = v/c$).

2. **Absorber-Eigenschaften $(Z, A, I)$:**
    * $Z/A$: Die Elektronendichte ($N_e = Z N_A / A$) des Absorbers bestimmt die Anzahl der Wechselwirkungspartner. (mit $Z$ = Ordnungszahl und $A$ = Massenzahl) Da $Z/A$ für die meisten Elemente nahe 0.5 liegt, variiert $S_{col}$ wenig zwischen verschiedenen Materialien.
    * $I$ (Mean Ionization/Excitation Energy): Die mittlere Ionisations-/Anregungsenergie. Dieser empirisch bestimmte Wert hängt nur vom Absorber ab und ist die minimale Energie $\Delta E_{min}$ für eine Wechselwirkung. Er wird in elektronenvolt (eV) angegeben.

3. **Relativistische Terme $\left( \ln \frac{\beta^2}{1-\beta^2} - \beta^2 \right)$:**
    * Diese Terme werden wichtig, wenn $\beta$ gegen 1 geht und führen zum langsamen Wiederanstieg der Bremskraft bei sehr hohen Energien.

`` Bild: BetheKorr ``

*Hinweis zu Korrekturen:* Um die Übereinstimmung mit Messdaten zu verbessern, insbesondere bei niedrigen Energien und in kondensierten Medien, werden der Bethe-Formel Korrekturen hinzugefügt: die **Shell Correction** $(C/Z)$ bei niedriger Energie (wenn Teilchengeschwindigkeit vergleichbar mit Elektronengeschwindigkeit ist) und die **Density Effect Correction** $(\delta)$ bei hohen Energien (aufgrund der Polarisierung des Mediums).


---

### 4. Die Form der Bethe Mass Collision Stopping Power Curve

Die Auftragung des Kollisionsbremsvermögens $S_{col}$ als Funktion der kinetischen Energie $E_K$ (für schwere geladene Teilchen) zeigt drei charakteristische Regionen [60, 61, Fig. 6.7]:

`` Bild: BetheCurve ``

#### Region 1: Niedrige Energie

* $S_{col}$ steigt mit $E_K$ an und erreicht ein Maximum ($S_{max}^{col}$).
* Die klassische Bethe-Theorie bricht hier ab, da die Annahme, dass das Teilchen schneller als die Orbitalelektronen ist, verletzt wird. Hier sind Shell-Korrekturen notwendig.
* Das Maximum tritt experimentell etwa bei $E_K \approx 250 I$ auf.

#### Region 2: Intermediäre Energie (MIP Region)

* Jenseits des Maximums fällt $S_{col}$ schnell ab, proportional zu $1/\beta^2$ (oder $1/E_K$).
* Dies folgt direkt aus dem dominanten $\beta^{-2}$-Term der Bethe-Gleichung.
* $S_{col}$ erreicht ein breites Minimum ($S_{min}^{col}$), das als **Minimum Ionizing Particle (MIP)**-Region bekannt ist.
* Das Minimum ist nahezu unabhängig vom Absorbermaterial und liegt bei $E_K \approx 2.5 M_0 c^2$.

#### Region 3: Relativistische Energie

* Jenseits des Minimums steigt $S_{col}$ langsam wieder an.
* Dieser Anstieg ist auf die relativistischen Terme der Bethe-Formel zurückzuführen $\left( \ln \frac{\beta^2}{1-\beta^2} \right)$.
* In kondensierten Medien wird dieser Anstieg durch den **Dichteeffekt** $(\delta)$ abgeschwächt oder gesättigt, da die Polarisation des Mediums die Reichweite der weichen Kollisionen begrenzt.


---

### 5. Makroskopische Konsequenzen: Der Bragg-Peak

Nachdem wir die mikroskopische und relativistische Theorie des Energieverlusts in Form der Bethe-Formel analysiert haben, betrachten wir nun die makroskopische Manifestation dieses Energieabgabezustands, insbesondere bei **schweren geladenen Teilchen** wie Protonen oder Alpha-Teilchen.

Der Energieverlust schwerer geladener Teilchen erfolgt nahezu ausschließlich durch Kollisionen ($S_{col}$). Da der Strahlungsverlust vernachlässigbar ist, bleiben diese Teilchen auf einem im Wesentlichen geradlinigen Pfad, bis sie zur Ruhe kommen.

`` Bild: BraggPeak ``

#### 5.1 Das Phänomen

Der **Bragg-Peak**, benannt nach William Henry Bragg, der ihn 1903 entdeckte, beschreibt den ausgeprägten Anstieg der Energiedepositionsrate (oder der Ionisationsdosis) am Ende des Teilchenpfades in einem absorbierenden Medium.

Dieser Peak ist die direkte Folge der Proportionalität der Kollisionsbremskraft zur reziproken Teilchengeschwindigkeit im intermediären Geschwindigkeitsbereich: $S_{col} \propto 1/\beta^2$.

*   **Mechanismus:** Während das Teilchen Materie durchquert und Energie verliert, verlangsamt es sich. Gemäß der Bethe-Formel führt diese Reduktion der Geschwindigkeit zu einem dramatischen Anstieg des Bremsvermögens $S_{col}$.
*   **Dosisabgabe:** Kurz bevor das schwere geladene Teilchen seine gesamte kinetische Energie $E_K$ verloren hat und zur Ruhe kommt, erreicht der Energieverlust pro Weglänge ($dE/dx$) ein Maximum, was zu einer hohen Dosisabgabe in dieser eng begrenzten Tiefe führt.

#### 5.2 Klinische Relevanz: Hadronentherapie

Die einzigartige Eigenschaft des Bragg-Peaks – nämlich die scharfe Abgrenzung der Dosisdeponierung in einer spezifischen Tiefe – ist der zentrale Vorteil der Hadronentherapie (Protonen- oder Schwerionentherapie) gegenüber der konventionellen Photonentherapie.

*   Im Gegensatz zu energiereichen Photonenstrahlen, deren Dosis exponentiell oder asymptotisch abfällt, erlaubt die Bragg-Peak-Kurve eine **millimetergenaue Dosierung** des Tumors, während das davor liegende Gewebe nur eine geringere Eintrittsdosis erhält und das dahinterliegende Gewebe nahezu vollständig geschont wird.

`` Bild: DSD_88 ``

*   **Anpassung des Peaks (SOBP):** Der Bragg-Peak eines monoenergetischen Strahls ist sehr schmal. Um größere Tumoren klinisch behandeln zu können, muss dieser Peak verbreitert werden. Dies wird durch die Erzeugung eines **Spread-Out Bragg Peak (SOBP)** erreicht, indem man einen Strahl mit einer verteilten Energie (variable Dicke von Abschwächern, sog. *spinning wedges*) verwendet. Die Modifikation des monoenergetischen Strahls resultiert in einem Plateau, das der spezifischen 3D-Form des Tumors angepasst werden kann.

`` Bild: SOBP ``

### 6. Zusammenfassung

Zusammenfassend lässt sich festhalten:

``klein neben Stichpunkten: Bild: 1920_hirntumorbestrahlung ``

Die **Wechselwirkungen geladener Teilchen mit Materie** sind durch zwei Hauptmechanismen definiert: den Kollisionsverlust ($S_{col}$) mit Orbitalelektronen und den Strahlungsverlust ($S_{rad}$) mit Atomkernen.

Das **Bremsvermögen $S$** ist die quantitative Beschreibung dieser Energieverlustrate.

Für schwere geladene Teilchen wird $S_{col}$ primär durch die **Bethe-Formel** beschrieben, welche die Abhängigkeit von der Teilchengeschwindigkeit über den $1/\beta^2$-Term und die Materialeigenschaften über die mittlere Ionisationsenergie $I$ darstellt. Die Bethe-Kurve zeigt einen $1/\beta^2$-Abfall bei mittleren Energien, gefolgt von einem Minimum (MIP-Region bei $E_K \approx 2.5 M_0 c^2$) und einem relativistischen Anstieg.

Die präzise Kenntnis dieser theoretischen Grundlagen, insbesondere der Dynamik des Energieverlusts, ermöglicht es uns, makroskopische Phänomene wie den **Bragg-Peak** zu modellieren.

Die Fähigkeit, den Bragg-Peak zu formen und präzise im Zielvolumen zu platzieren, ist die technologische und physikalische Errungenschaft, die die moderne **Hadronentherapie** definiert und die Grundlage für die Dosimetrie in der Medizinphysik bildet. Die Forschung in diesem Bereich ist weiterhin essenziell, um die klinische Präzision fortlaufend zu optimieren.

``Bild: 1920_hirntumorbestrahlung `` ``Text: Abschlussfolie: Titel & Florian Adamczyk ``

Ich danke Ihnen für Ihre Aufmerksamkeit und stehe nun für Fragen zur Verfügung.