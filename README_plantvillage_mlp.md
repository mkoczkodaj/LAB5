# PlantVillage MLP PyTorch - instrukcja

Plik główny: `plantvillage_mlp_pytorch_lab.ipynb`

## Dane

Pobierz dataset z Kaggle:

https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset

Rozpakuj go tak, aby notebook widział jeden z katalogów:

- `plantvillage-dataset/plantvillage dataset/color`
- `plantvillage dataset/color`
- `PlantVillage`
- `data/plantvillage dataset/color`
- `data/PlantVillage`

Jeżeli katalog jest inny, ustaw w pierwszej komórce:

```python
DATA_DIR = Path("twoja/sciezka/do/katalogu_z_klasami")
```

## Co zawiera notebook

- wybór co najmniej 5 klas z PlantVillage,
- podział train/validation/test ze stratyfikacją,
- MLP z jedną warstwą ukrytą,
- MLP z drugą warstwą ukrytą,
- testy `batch_size`, `optimizer`, `lr`, `dropout`, `weight_decay`, `batchnorm`, augmentacji i aktywacji,
- wykresy loss/accuracy,
- confusion matrix i classification report,
- tabela końcowa z hiperparametrami i dokładnością,
- eksport tabeli do `plantvillage_mlp_results.csv`,
- mały CNN do wizualizacji filtrów splotowych.

## Uwaga do sprawozdania

Czysty MLP nie ma filtrów splotowych, bo obraz jest spłaszczany do wektora. Dlatego wizualizacja filtrów w notebooku jest wykonana dla dodatkowego modelu CNN, a główne porównanie hiperparametrów dotyczy MLP.
