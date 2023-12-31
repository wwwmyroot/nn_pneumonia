# nn_pneumonia
NN for pneumonia detection

------

**Разработка нейросети для обнаружения пневмонии на флюрограммах.**

* Основной код (.py) - [NN_pneumonia_MAIN.py](https://github.com/wwwmyroot/nn_pneumonia/blob/main/NN_pneumonia_MAIN.py)
* Ноутбук (.ipynb) - [NN_pneumonia_MAIN.ipynb](https://github.com/wwwmyroot/nn_pneumonia/blob/main/NN_pneumonia_MAIN.ipynb)
* Ноутбук с output cells  (GoogleCollab) - [NN_pneumonia_MAIN_with_output.ipynb](https://github.com/wwwmyroot/nn_pneumonia/blob/main/NN_pneumonia_MAIN_with_output.ipynb)
* Скрины - в папке [/img](https://github.com/wwwmyroot/nn_pneumonia/tree/main/img)

-----

* **Dataset:** yandexcloud, 1.06G _ chest_xray.zip

-----

* **Results:**

- **Эксп. №1**
  - Средняя точность на обучающей выборке: 0.981
  - Максимальная точность на обучающей выборке: 0.983
  - Средняя точность на проверочной выборке: 0.972
  - Максимальная точность на проверочной выборке: 0.975

- **Эксп. №2 (убран макс-пуллинг)**
  - Средняя точность на обучающей выборке: 1.0
  - Максимальная точность на обучающей выборке: 1.0
  - Средняя точность на проверочной выборке: 0.97
  - Максимальная точность на проверочной выборке: 0.974
  
- **Эксп. №3 (добавлен полносвязный слой в конце)**
  - Средняя точность на обучающей выборке: 0.989
  - Максимальная точность на обучающей выборке: 0.991
  - Средняя точность на проверочной выборке: 0.973
  - Максимальная точность на проверочной выборке: 0.979
  
- **Эксп. №4 (усилен полносвязный слой в конце)**
  - Средняя точность на обучающей выборке: 0.993
  - Максимальная точность на обучающей выборке: 0.995
  - Средняя точность на проверочной выборке: 0.973
  - Максимальная точность на проверочной выборке: 0.975

- **Эксп. №5 (ослаблен полносвязный слой в конце)**
  - Средняя точность на обучающей выборке: 0.984
  - Максимальная точность на обучающей выборке: 0.985
  - Средняя точность на проверочной выборке: 0.972
  - Максимальная точность на проверочной выборке: 0.973

- **Эксп. №6 (ослаблен первый сверточный слой)**
  - Средняя точность на обучающей выборке: 0.986
  - Максимальная точность на обучающей выборке: 0.989
  - Средняя точность на проверочной выборке: 0.974
  - Максимальная точность на проверочной выборке: 0.975

- **Эксп. №7 (усилен первый сверточный слой)**
  - Средняя точность на обучающей выборке: 0.993
  - Максимальная точность на обучающей выборке: 0.995
  - Средняя точность на проверочной выборке: 0.974
  - Максимальная точность на проверочной выборке: 0.976

- **Эксп. №8 (усилен второй сверточный)**
  - Средняя точность на обучающей выборке: 1.0
  - Максимальная точность на обучающей выборке: 1.0
  - Средняя точность на проверочной выборке: 0.978
  - Максимальная точность на проверочной выборке: 0.979

- **Эксп. №9 (добавление третьего сверточного блока)**
  - Средняя точность на обучающей выборке: 1.0
  - Максимальная точность на обучающей выборке: 1.0
  - Средняя точность на проверочной выборке: 0.976
  - Максимальная точность на проверочной выборке: 0.978

- **Эксп. №10 (добавление четвертого сверточного блока)**
  - Средняя точность на обучающей выборке: 1.0
  - Максимальная точность на обучающей выборке: 1.0
  - Средняя точность на проверочной выборке: 0.976
  - Максимальная точность на проверочной выборке: 0.977

- **Эксп. №11 (добавление BatchNorm + Dropout)**
  - Средняя точность на обучающей выборке: 1.0
  - Максимальная точность на обучающей выборке: 1.0
  - Средняя точность на проверочной выборке: 0.985
  - Максимальная точность на проверочной выборке: 0.986

- **Эксп. №12 (Переход на 128х128)**
  - Средняя точность на обучающей выборке: 1.0
  - Максимальная точность на обучающей выборке: 1.0
  - Средняя точность на проверочной выборке: 0.988
  - Максимальная точность на проверочной выборке: 0.989

- **Эксп. №13 (Смена ядра сверточного слоя)**
  - Средняя точность на обучающей выборке: 1.0
  - Максимальная точность на обучающей выборке: 1.0
  - Средняя точность на проверочной выборке: 0.988
  - Максимальная точность на проверочной выборке: 0.99

- **Эксп. №14 (Смена ядра 2 и последующих сверточных слоев)**
  - Средняя точность на обучающей выборке: 1.0
  - Максимальная точность на обучающей выборке: 1.0
  - Средняя точность на проверочной выборке: 0.985
  - Максимальная точность на проверочной выборке: 0.987

----- 

**Дополнительно. Перечень опробованных предобученных моделей.**

- Эксп. №1 NASNetMobile (99.3%)
- Эксп. №2 ResNet50 (99.04%)
- Эксп. №3 ResNet50v2 (99.1%)
- Эксп. №4 VGG16 (98.9%)
- Эксп. №5 VGG19 (98.8%)
- Эксп. №6 XCeption (99.4%)

-----
 

