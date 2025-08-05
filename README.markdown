# Handel akcjami z wykorzystaniem uczenia ze wzmocnieniem

To repozytorium zawiera dwa notatniki Jupyter, które demonstrują zastosowanie algorytmów uczenia ze wzmocnieniem do handlu akcjami. Zaimplementowane algorytmy to Proximal Policy Optimization (PPO) oraz Deep Q-Network (DQN). Notatniki wykorzystują historyczne dane giełdowe oraz techniki uczenia ze wzmocnieniem do stworzenia agentów handlowych, którzy podejmują decyzje kupna lub sprzedaży na podstawie zdefiniowanych wskaźników i warunków rynkowych.

## Notatniki

### 1. PPO_z_score_indeksy.ipynb
Ten notatnik implementuje strategię handlową z użyciem algorytmu Proximal Policy Optimization (PPO). Zawiera następujące kroki:
- **Ładowanie danych:** Wczytywane są historyczne dane giełdowe dla kilku spółek (np. Intel, IBM, Nvidia).
- **Konfiguracja środowiska:** Tworzone jest niestandardowe środowisko handlowe przy użyciu pakietu `gym-anytrading`, z uwzględnieniem wskaźników takich jak RSI i SMA.
- **Trenowanie agenta PPO:** Algorytm PPO jest używany do trenowania agenta na podstawie danych giełdowych.
- **Ewaluacja:** Wyniki wyszkolonego agenta są oceniane i wizualizowane.

### 2. DQN_z_score_indeksy.ipynb
Ten notatnik implementuje strategię handlową z użyciem algorytmu Deep Q-Network (DQN). Struktura notatnika jest podobna do notatnika PPO:
- **Ładowanie danych:** Wykorzystywane są te same dane giełdowe.
- **Konfiguracja środowiska:** Środowisko jest przygotowywane w sposób kompatybilny z algorytmem DQN.
- **Trenowanie agenta DQN:** Algorytm DQN jest używany do trenowania agenta handlowego.
- **Ewaluacja:** Wyniki agenta są analizowane i porównywane z podejściem PPO.

## Wymagania

Aby uruchomić notatniki, należy zainstalować następujące pakiety Pythona:

- `pandas`
- `numpy`
- `matplotlib`
- `gym`
- `gym-anytrading`
- `stable-baselines3`
- `talib`
- `torch`

Możesz zainstalować te zależności za pomocą pip:

```bash
pip install pandas numpy matplotlib gym gym-anytrading stable-baselines3 ta-lib torch
```

## Uruchamianie notatników

1. Sklonuj repozytorium:

```bash
git clone https://github.com/yourusername/stock-trading-rl.git
cd stock-trading-rl
```

2. Uruchom Jupyter Notebook:

```bash
jupyter notebook
```

3. Otwórz wybrany notatnik (`PPO_z_score_indeksy.ipynb` lub `DQN_z_score_indeksy.ipynb`) i uruchom komórki sekwencyjnie.

## Wyniki

Notatniki zawierają wizualizacje i statystyki, które pokazują wyniki agentów PPO i DQN w symulowanych scenariuszach handlu akcjami. Obejmują one analizę zysków/strat, sumę nagród oraz działania handlowe (punkty kupna/sprzedaży).

