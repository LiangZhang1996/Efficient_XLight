# Efficient XLights
## 1、Introduction
The code for article **Efficient Pressure: Improving efficiency for signalized intersections**.

## 2、Requirements

`python3.6`,`tensorflow=2.4`, `cityflow`, `pandas`, `numpy`

[`cityflow`](https://github.com/cityflow-project/CityFlow.git) needs a linux environment, and we run the code on Manjaro Linux.

## 3、Usage

Parameters are well prepared so you can run the code directly.


For `Efficient-PressLight`, run:
```shell
python run_efficient_presslight.py
```

For `Efficient-CoLight`, run:
```shell
python run_efficient_colight.py
```

For `Efficient-MPLight`, run:
```shell
python run_efficient_mplight.py
```


For the baseline methods,
- Fixed-Time
```shell
python run_fixedtime.py
```
- Max-Pressure
```shell
python run_maxpressure.py
```
- PressLight
```shell
python run_presslight.py
```
- MPLight
```shell
python run_mplight.py
```
- Colight
```shell
python run_colight.py
```


## 4、Code details
### 4.1、structure
- `models`: contains all the models used in our article.
- `utils`: contains all the methods to simulate and train the models.

### 4.2、Reference

The code is modified from [MPLight](https://github.com/Chacha-Chen/MPLight.git). 

The `Max-Pressure` is created by ourselves, based on [MaxPressure](https://www.sciencedirect.com/science/article/pii/S0968090X13001782) .
- `PressLight`: Bsed on `LIT` model, which comes from [Colight](https://github.com/wingsweihua/colight.git).
- `Colight` : Based on [Colight](https://github.com/wingsweihua/colight.git).
- `Fixed-Time`: From [MPLight](https://github.com/Chacha-Chen/MPLight.git).
- `MPLight`: From [MPLight](https://github.com/Chacha-Chen/MPLight.git).

If you use our method and code, please cite our article.
