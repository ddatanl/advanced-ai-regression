# Advanced AI: Regressie: Zelf aan de slag met notebooks

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ddatanl/advanced-ai-regression/main)

Interactieve notebooks bij de eendaagse training **Regressie & Voorspellende Modellen** van D-Data.
Van lineaire regressie tot random forest, met telkens een korte, praktische opdracht.

De map is opgesplitst in:

- `opdrachten/` → opdrachten voor deelnemers (met `# TODO`'s om in te vullen)
- `antwoorden/` → volledige uitwerkingen voor trainer of zelfcontrole

## Leerroute (aanbevolen volgorde)

De opdrachten volgen de blokken van de training en bouwen op elkaar voort.

| # | Opdracht | Onderwerp | Duur |
|---|----------|-----------|------|
| 1 | `Opdracht1_Verkenning_cursist.ipynb` | Dataset verkennen, train/test-split, baseline, MAE/RMSE/R² | ~20 min |
| 2 | `Opdracht2_LineairModel_cursist.ipynb` | Lineair model, coëfficiënten, residuenplot, VIF, Ridge | ~30 min |
| 3 | `Opdracht3_Logistisch_cursist.ipynb` | Logistische regressie, confusion matrix, ROC/AUC, odds ratio | ~30 min |
| 4 | `Opdracht4_TimeSeries_cursist.ipynb` | Tijdreeks, lag-features, time-based split, naïeve baseline | ~30 min |
| 5 | `Opdracht5_Trees_cursist.ipynb` | Decision tree, random forest, feature importance, overfitting | ~30 min |
| 6 | `Capstone_cursist.ipynb` | Volledige workflow toepassen op een eigen dataset | rest van de middag |

De uitwerkingen staan onder dezelfde naam in `antwoorden/` (met `_antwoordmodel` in plaats van `_cursist`).

## Oefenen

| Type | Map | Doel |
|---|---|---|
| Opdracht | `opdrachten/` | Deelnemers vullen zelf de `# TODO`'s in; de rest staat klaar |
| Antwoorden | `antwoorden/` | Volledige uitwerking met toelichting voor de trainer |

## Starten

### Optie 1: Binder (geen installatie nodig)

Klik op de Binder-badge bovenaan deze README. Het kan 1-2 minuten duren voordat de omgeving is opgestart.
Binder bouwt de omgeving automatisch op basis van `requirements.txt`.

### Optie 2: Lokaal

```bash
# 1. (optioneel) maak een virtuele omgeving
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate

# 2. installeer de benodigde packages
pip install -r requirements.txt

# 3. start JupyterLab
jupyter lab
```

Open daarna het notebook dat de trainer aangeeft, te beginnen met
`opdrachten/Opdracht1_Verkenning_cursist.ipynb`.

## Instructies voor deelnemers

1. Klik op de Binder-link die je van de trainer hebt gekregen (of start lokaal — zie hierboven).
2. Wacht tot de omgeving is opgestart.
3. Open het notebook dat de trainer aangeeft (begin bij opdracht 1).
4. Lees de tekst boven elke cel en voer de cellen op volgorde uit met **Shift + Enter**.
5. Vul de plekken met **`# TODO`** zelf in — dat zijn de kernstappen van de opdracht.
6. De overige cellen zijn al ingevuld; die hoef je alleen uit te voeren.
7. Loop je vast? Kijk in de bijbehorende uitwerking in de map `antwoorden/`.

> **Let op:** Binder-sessies verlopen na ~10 minuten inactiviteit. Sla je werk dus tussentijds op
> (download je notebook), want wijzigingen blijven niet bewaard in Binder.

## Opmerkingen

- Alle notebooks draaien **zonder GPU** en gebruiken uitsluitend `numpy`, `pandas`, `matplotlib` en `scikit-learn`.
- De datasets zitten **ingebouwd in scikit-learn** of worden in het notebook zelf gegenereerd — je hoeft niets te downloaden. Daardoor werken de notebooks ook prima in Binder en offline.
- Aanbevolen: Python 3.10 of nieuwer.
