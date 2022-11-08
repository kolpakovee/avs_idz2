# avs_idz2
Здравствуйте, дорогие проверяющие! 

Это ИДЗ №2 по АВС студента БПИ215 Колпакова Егора Евгеньевича. 

Мой вариант 19 представлен ниже:

![variant](https://github.com/kolpakovee/avs_idz2/blob/main/вариант.png)

---
**Формат ввода:**
- Вводится строка, содержащая n (n <= 1 000 000) символов только из первой половины ASCII-таблицы (коды в диапазоне 0–127), затем НЕОБХОДИМО нажать ctrl + D! Так обозначается конец ввода. 
---
**Формат вывода.**
- Для каждого отображаемого (ASCII-код >= 32) символа из вводимой строки выводится число k, которое показывает сколько раз этот символ встречался в строке. Затем выводится число m - кол-во различный отображаемых символов в строке. Например для строки "Egor" вывод будет:
```
E => 1
g => 1
o => 1
r => 1
4
```
---
## 4 балла
![4_1](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/4_1.png)
 - В проекте это файл main.c
---
![4_2](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/4_2.png)

- Компиляция без отладочных опций:

![compilation1](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/compilation1.png)

- После компиляции создался файл first.s, комментарии написаны в нём
---

![4_3](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/4_3.png)

- Использованы аргументы командой строки и ручное редактирование, получился файл second.s

![compilation2](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/compilation2.png)

---
![4_4](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/4_4.png)

- Программа скомпилирована и скомпонована без опций отладки
![compilation3](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/compilation3)

---
![4_5](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/4_5.png)

**Тесты**

*Предполагается, что все введённые числа будут >= 0 и <= 10000, так как длин сторон квадрата, так же предполагается, что длина массива А >= 0.*

1) Ввод: 
```
I love C#!
```

Предполагаемый вывод:
```
  => 2
! => 1
# => 1
C => 1
I => 1
e => 1
l => 1
o => 1
v => 1
9
```

Вывод программы на C:

```
  => 2
! => 1
# => 1
C => 1
I => 1
e => 1
l => 1
o => 1
v => 1
9
```

Вывод программы на GAS:

```
  => 2
! => 1
# => 1
C => 1
I => 1
e => 1
l => 1
o => 1
v => 1
9
```
---
2) Ввод: 
```
0
```

Предполагаемый вывод:
```
ArrayB: 
```

Вывод программы на C:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test2C.png)

Вывод программы на GAS:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test2GAS.png)
---
3) Ввод: 
```
1001
```

Предполагаемый вывод:
```
You entered an invalid number.
```

Вывод программы на C:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test3C.png)

Вывод программы на GAS:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test3GAS.png)
---
4) Ввод: 
```
10
6807 5249 73 3658 8930 1272 7544 878 7923 7709
```

Предполагаемый вывод:
```
ArrayB: 46335249 27552001 5329 13380964 79744900 1617984 56911936 770884 62773929 59428681
```

Вывод программы на C:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test4C.png)

Вывод программы на GAS:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test4GAS.png)
---
5) Ввод: 
```
100
7806 6248 1072 4657 9929 2271 8543 1877 8922 8708 5439 9164 5491 4041 8986 3502 3326 2728 9839 3611 5302 4168 8708 8156 559 1932 4098 1277 2815 6334 96 8825 4511 266 4809 8632 1978 148 7578 9820 2966 1671 2392 335 6484 2744 6227 5090 1193 7356 6000 2152 7707 8943 6667 2489 9123 3195 529 1902 8721 5665 9548 9023 8800 7852 1976 8407 9227 5932 1297 9980 9634 9012 4864 813 62 5535 424 2668 5114 1093 6628 7500 7516 5194 1104 1403 450 5297 3187 2122 504 7881 7751 2565 7715 1336 5437 4143 
```

Предполагаемый вывод:
```
ArrayB: 60933636 39037504 1149184 21687649 98585041 5157441 72982849 3523129 79602084 75829264 29582721 83978896 30151081 16329681 80748196 12264004 11062276 7441984 96805921 13039321 28111204 17372224 75829264 66520336 312481 3732624 16793604 1630729 7924225 40119556 9216 77880625 20349121 70756 23126481 74511424 3912484 21904 57426084 96432400 8797156 2792241 5721664 112225 42042256 7529536 38775529 25908100 1423249 54110736 36000000 4631104 59397849 79977249 44448889 6195121 83229129 10208025 279841 3617604 76055841 32092225 91164304 81414529 77440000 61653904 3904576 70677649 85137529 35188624 1682209 99600400 92813956 81216144 23658496 660969 3844 30636225 179776 7118224 26152996 1194649 43930384 56250000 56490256 26977636 1218816 1968409 202500 28058209 10156969 4502884 254016 62110161 60078001 6579225 59521225 1784896 29560969 17164449
```

Вывод программы на C:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test5C.png)

Вывод программы на GAS:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test5GAS.png)
---
6) Ввод: 
```
1
1
```

Предполагаемый вывод:
```
ArrayB: 1
```

Вывод программы на C:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test6C.png)

Вывод программы на GAS:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test6GAS.png)
---
7) Ввод: 
```
5
0 0 0 0 0
```

Предполагаемый вывод:
```
ArrayB: 0 0 0 0 0
```

Вывод программы на C:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test7C.png)

Вывод программы на GAS:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test7GAS.png)
---
8) Ввод: 
```
1
999
```

Предполагаемый вывод:
```
ArrayB: 998001
```

Вывод программы на C:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test8C.png)

Вывод программы на GAS:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test8GAS.png)
---
9) Ввод: 
```
500
7140 5582 406 3991 9263 1605 7877 1211 8256 8042 4773 8498 4825 3375 8320 2836 2660 2062 9173 2945 4636 3502 8042 7490 9893 1266 3432 611 2149 5668 9430 8159 3845 9600 4143 7966 1312 9482 6912 9154 2300 1005 1726 9669 5818 2078 5561 4424 527 6690 5334 1486 7041 8277 6001 1823 8457 2529 9863 1236 8055 4999 8882 8357 8134 7186 1310 7741 8561 5266 631 9314 8968 8346 4198 147 9396 4869 9758 2002 4448 427 5962 6834 6850 4528 438 737 9784 4631 2521 1456 9838 7215 7085 1899 7049 670 4771 3477 1834 5230 4204 6161 1470 9691 3510 2730 2627 8237 1942 6564 78 4508 3968 6631 8475 732 8301 745 593 3890 1927 8341 6728 6301 9446 4863 1339 1295 8275 5698 2415 185 1100 4154 6028 5045 4004 234 8923 5164 5071 3390 1949 123 5973 1012 7668 7339 8305 6431 9428 5652 3787 5556 2622 7093 9238 6459 6456 9839 6146 7103 5571 9427 6553 8177 2699 867 5559 5727 1696 9071 8177 9923 6883 5492 8956 5280 7718 7550 5605 5872 9580 2718 3829 5218 956 2753 8477 2301 6068 248 1958 3867 6375 6344 5012 4485 5577 7628 9151 729 8025 2148 3324 366 3002 9730 9886 880 6158 1543 9995 544 4141 3710 3094 958 7668 2201 8328 3109 3100 7772 207 9664 889 6634 9205 893 427 9317 4088 122 1740 8348 526 3102 6013 3788 7188 7839 1296 3835 7009 3441 3582 2664 8177 7971 1141 330 8984 5182 5536 6064 6864 8347 5752 7108 2342 513 8262 5556 4387 8593 7070 1878 7650 7858 4533 4589 1897 930 6981 8037 5883 5483 2309 1745 8887 3130 2837 8714 5081 7398 9711 8032 8542 5462 8886 5816 780 4940 1106 5655 4638 5509 386 7557 4963 699 5733 777 5703 618 3349 4231 8488 1466 5890 6909 3511 8599 7690 2044 8211 947 5152 6070 3466 924 4053 9095 6966 6530 6364 8921 922 5206 9210 7637 9691 1533 7587 9293 5248 4280 5813 8063 288 4879 7440 1571 333 5259 5368 5190 1446 447 9926 1693 8687 8751 5690 2918 4062 1348 6896 6435 1250 6976 9752 3300 8080 5602 5728 3636 4806 9436 2081 4718 5991 3792 5739 4263 157 5465 1306 9936 7230 8253 4283 5564 8813 536 4233 4853 2866 1591 7336 9009 1283 4267 9113 212 2165 2907 3882 4875 6582 3104 6643 6212 1316 303 2373 3056 3983 3304 3562 651 8079 632 7563 5954 1109 457 8577 7291 8029 7104 9397 1893 6931 9084 273 4836 9884 3134 7538 5413 751 9607 9982 746 3653 9358 2345 2116 5121 4450 4341 1883 5657 9528 1590 4844 6023 8999 2743 926 886 9898 1293 9075 1736 4685 7640 6474 5243 3533 3132 3460 504 8120 4747 1958 6974 9850 5681 2175 4648 6307 1778 1706 2553 244 9572 5387 1638 7262 2586 4522 5499 4689 9637 193 6231 5925 2053 6449 1913 9200 9685 7272 9031 5234 
```

Предполагаемый вывод:
```
ArrayB: 50979600 31158724 164836 15928081 85803169 2576025 62047129 1466521 68161536 64673764 22781529 72216004 23280625 11390625 69222400 8042896 7075600 4251844 84143929 8673025 21492496 12264004 64673764 56100100 97871449 1602756 11778624 373321 4618201 32126224 88924900 66569281 14784025 92160000 17164449 63457156 1721344 89908324 47775744 83795716 5290000 1010025 2979076 93489561 33849124 4318084 30924721 19571776 277729 44756100 28451556 2208196 49575681 68508729 36012001 3323329 71520849 6395841 97278769 1527696 64883025 24990001 78889924 69839449 66161956 51638596 1716100 59923081 73290721 27730756 398161 86750596 80425024 69655716 17623204 21609 88284816 23707161 95218564 4008004 19784704 182329 35545444 46703556 46922500 20502784 191844 543169 95726656 21446161 6355441 2119936 96786244 52056225 50197225 3606201 49688401 448900 22762441 12089529 3363556 27352900 17673616 37957921 2160900 93915481 12320100 7452900 6901129 67848169 3771364 43086096 6084 20322064 15745024 43970161 71825625 535824 68906601 555025 351649 15132100 3713329 69572281 45265984 39702601 89226916 23648769 1792921 1677025 68475625 32467204 5832225 34225 1210000 17255716 36336784 25452025 16032016 54756 79619929 26666896 25715041 11492100 3798601 15129 35676729 1024144 58798224 53860921 68973025 41357761 88887184 31945104 14341369 30869136 6874884 50310649 85340644 41718681 41679936 96805921 37773316 50452609 31036041 88868329 42941809 66863329 7284601 751689 30902481 32798529 2876416 82283041 66863329 98465929 47375689 30162064 80209936 27878400 59567524 57002500 31416025 34480384 91776400 7387524 14661241 27227524 913936 7579009 71859529 5294601 36820624 61504 3833764 14953689 40640625 40246336 25120144 20115225 31102929 58186384 83740801 531441 64400625 4613904 11048976 133956 9012004 94672900 97732996 774400 37920964 2380849 99900025 295936 17147881 13764100 9572836 917764 58798224 4844401 69355584 9665881 9610000 60403984 42849 93392896 790321 44009956 84732025 797449 182329 86806489 16711744 14884 3027600 69689104 276676 9622404 36156169 14348944 51667344 61449921 1679616 14707225 49126081 11840481 12830724 7096896 66863329 63536841 1301881 108900 80712256 26853124 30647296 36772096 47114496 69672409 33085504 50523664 5484964 263169 68260644 30869136 19245769 73839649 49984900 3526884 58522500 61748164 20548089 21058921 3598609 864900 48734361 64593369 34609689 30063289 5331481 3045025 78978769 9796900 8048569 75933796 25816561 54730404 94303521 64513024 72965764 29833444 78960996 33825856 608400 24403600 1223236 31979025 21511044 30349081 148996 57108249 24631369 488601 32867289 603729 32524209 381924 11215801 17901361 72046144 2149156 34692100 47734281 12327121 73942801 59136100 4177936 67420521 896809 26543104 36844900 12013156 853776 16426809 82719025 48525156 42640900 40500496 79584241 850084 27102436 84824100 58323769 93915481 2350089 57562569 86359849 27541504 18318400 33790969 65011969 82944 23804641 55353600 2468041 110889 27657081 28815424 26936100 2090916 199809 98525476 2866249 75463969 76580001 32376100 8514724 16499844 1817104 47554816 41409225 1562500 48664576 95101504 10890000 65286400 31382404 32809984 13220496 23097636 89038096 4330561 22259524 35892081 14379264 32936121 18173169 24649 29866225 1705636 98724096 52272900 68112009 18344089 30958096 77668969 287296 17918289 23551609 8213956 2531281 53816896 81162081 1646089 18207289 83046769 44944 4687225 8450649 15069924 23765625 43322724 9634816 44129449 38588944 1731856 91809 5631129 9339136 15864289 10916416 12687844 423801 65270241 399424 57198969 35450116 1229881 208849 73564929 53158681 64464841 50466816 88303609 3583449 48038761 82519056 74529 23386896 97693456 9821956 56821444 29300569 564001 92294449 99640324 556516 13344409 87572164 5499025 4477456 26224641 19802500 18844281 3545689 32001649 90782784 2528100 23464336 36276529 80982001 7524049 857476 784996 97970404 1671849 82355625 3013696 21949225 58369600 41912676 27489049 12482089 9809424 11971600 254016 65934400 22534009 3833764 48636676 97022500 32273761 4730625 21603904 39778249 3161284 2910436 6517809 59536 91623184 29019769 2683044 52736644 6687396 20448484 30239001 21986721 92871769 37249 38825361 35105625 4214809 41589601 3659569 84640000 93799225 52881984 81558961 27394756
```

Вывод программы на C:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test9C.png)

Вывод программы на GAS:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test9GAS.png)
---
10) Ввод: 
```
1000
3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 
```

Предполагаемый вывод:
```
ArrayB: 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 
```

Вывод программы на C:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test10C.png)

Вывод программы на GAS:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test10GAS.png)

---
Прошу прощения за огромное кол-во чисел, но я хотел показать, что программа работает корректно.

---
![4_6](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/4_6.png)

- Отчёт сформирован.
---
## 5 баллов
![5_1](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/5_1.png)

- Функции с передачей данных через параметры использованы (файл main.c)

```
void getArrayA(int sizeA){  
    for (int i = 0; i < sizeA; ++i) {  
        int value;  
        printf("Enter %d value: ", i + 1);  
        scanf("%d", &value);  
        arrayA[i] = value;  
    }  
}  
  
void getArrayB(int sizeA){  
    for (int i = 0; i < sizeA; ++i) {  
        arrayB[i] = arrayA[i] * arrayA[i];  
    }  
}  
  
void outResult(int sizeA){  
    printf("Array B: ");  
    for (int i = 0; i < sizeA; ++i) {  
        printf("%d ",arrayB[i]);  
    }  
}
```

---
![5_2](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/5_2.png)

- Локальные переменные использованы(Например, value в функции getArrayA и sizeA в функции main). Это можно увидеть в файле main.c
```
int value;

int sizeA;
```
---
![5_3](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/5_3.png)
-   В ассемблерную программу при вызове функции добавлены комментарии, описывающие передачу фактических параметров и перенос возвращаемого результата. Это можно увидеть в файле second.s
---
![5_4](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/5_4.png)
-    В функциях для формальных параметров добавлены комментарии, описывающие связь между параметрами языка Си и регистрами (стеком). Это можно увидеть в фале second.s
---
![5_5](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/5_5.png)

- Информация добавлена в отчёт

## 6 баллов
![6_1](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/6_1.png)

- Произведёе рефакторинг программы, все изменения можно увидеть в файле optimized.s:
 1) DWORD PTR -4[rbp] заменено на r12d (переменную цикла i теперь храним в регистре r12d)
2) загрузили переменную sizeA в регистр r13d и DWORD PTR -4[rbp] заменено на r13d
3) DWORD PTR -20[rbp] заменено r14d
4) загрузили переменную value в регистр r15d и DWORD PTR -8[rbp] заменено r15d

 - Чтобы увидеть все изменения можно сравнить файлы second.s и optimized.s!

---
![6_2](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/6_2.png)
- Комментарии добавлены в файл optimized.s
---
![6_3](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/6_3.png)

1) Ввод: 
```
10 
1 2 3 4 5 6 7 8 9 10
```

Предполагаемый вывод:
```
ArrayB: 1 4 9 25 36 49 64 81 100
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test1C.png)

---
2) Ввод: 
```
0
```

Предполагаемый вывод:
```
ArrayB: 
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test2C.png)

---
3) Ввод: 
```
1001
```

Предполагаемый вывод:
```
You entered an invalid number.
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test3C.png)

---
4) Ввод: 
```
10
6807 5249 73 3658 8930 1272 7544 878 7923 7709
```

Предполагаемый вывод:
```
ArrayB: 46335249 27552001 5329 13380964 79744900 1617984 56911936 770884 62773929 59428681
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test4C.png)

---
5) Ввод: 
```
100
7806 6248 1072 4657 9929 2271 8543 1877 8922 8708 5439 9164 5491 4041 8986 3502 3326 2728 9839 3611 5302 4168 8708 8156 559 1932 4098 1277 2815 6334 96 8825 4511 266 4809 8632 1978 148 7578 9820 2966 1671 2392 335 6484 2744 6227 5090 1193 7356 6000 2152 7707 8943 6667 2489 9123 3195 529 1902 8721 5665 9548 9023 8800 7852 1976 8407 9227 5932 1297 9980 9634 9012 4864 813 62 5535 424 2668 5114 1093 6628 7500 7516 5194 1104 1403 450 5297 3187 2122 504 7881 7751 2565 7715 1336 5437 4143 
```

Предполагаемый вывод:
```
ArrayB: 60933636 39037504 1149184 21687649 98585041 5157441 72982849 3523129 79602084 75829264 29582721 83978896 30151081 16329681 80748196 12264004 11062276 7441984 96805921 13039321 28111204 17372224 75829264 66520336 312481 3732624 16793604 1630729 7924225 40119556 9216 77880625 20349121 70756 23126481 74511424 3912484 21904 57426084 96432400 8797156 2792241 5721664 112225 42042256 7529536 38775529 25908100 1423249 54110736 36000000 4631104 59397849 79977249 44448889 6195121 83229129 10208025 279841 3617604 76055841 32092225 91164304 81414529 77440000 61653904 3904576 70677649 85137529 35188624 1682209 99600400 92813956 81216144 23658496 660969 3844 30636225 179776 7118224 26152996 1194649 43930384 56250000 56490256 26977636 1218816 1968409 202500 28058209 10156969 4502884 254016 62110161 60078001 6579225 59521225 1784896 29560969 17164449
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test5C.png)

---
6) Ввод: 
```
1
1
```

Предполагаемый вывод:
```
ArrayB: 1
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test6C.png)

---
7) Ввод: 
```
5
0 0 0 0 0
```

Предполагаемый вывод:
```
ArrayB: 0 0 0 0 0
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test7C.png)

---
8) Ввод: 
```
1
999
```

Предполагаемый вывод:
```
ArrayB: 998001
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test8C.png)

---
9) Ввод: 
```
500
7140 5582 406 3991 9263 1605 7877 1211 8256 8042 4773 8498 4825 3375 8320 2836 2660 2062 9173 2945 4636 3502 8042 7490 9893 1266 3432 611 2149 5668 9430 8159 3845 9600 4143 7966 1312 9482 6912 9154 2300 1005 1726 9669 5818 2078 5561 4424 527 6690 5334 1486 7041 8277 6001 1823 8457 2529 9863 1236 8055 4999 8882 8357 8134 7186 1310 7741 8561 5266 631 9314 8968 8346 4198 147 9396 4869 9758 2002 4448 427 5962 6834 6850 4528 438 737 9784 4631 2521 1456 9838 7215 7085 1899 7049 670 4771 3477 1834 5230 4204 6161 1470 9691 3510 2730 2627 8237 1942 6564 78 4508 3968 6631 8475 732 8301 745 593 3890 1927 8341 6728 6301 9446 4863 1339 1295 8275 5698 2415 185 1100 4154 6028 5045 4004 234 8923 5164 5071 3390 1949 123 5973 1012 7668 7339 8305 6431 9428 5652 3787 5556 2622 7093 9238 6459 6456 9839 6146 7103 5571 9427 6553 8177 2699 867 5559 5727 1696 9071 8177 9923 6883 5492 8956 5280 7718 7550 5605 5872 9580 2718 3829 5218 956 2753 8477 2301 6068 248 1958 3867 6375 6344 5012 4485 5577 7628 9151 729 8025 2148 3324 366 3002 9730 9886 880 6158 1543 9995 544 4141 3710 3094 958 7668 2201 8328 3109 3100 7772 207 9664 889 6634 9205 893 427 9317 4088 122 1740 8348 526 3102 6013 3788 7188 7839 1296 3835 7009 3441 3582 2664 8177 7971 1141 330 8984 5182 5536 6064 6864 8347 5752 7108 2342 513 8262 5556 4387 8593 7070 1878 7650 7858 4533 4589 1897 930 6981 8037 5883 5483 2309 1745 8887 3130 2837 8714 5081 7398 9711 8032 8542 5462 8886 5816 780 4940 1106 5655 4638 5509 386 7557 4963 699 5733 777 5703 618 3349 4231 8488 1466 5890 6909 3511 8599 7690 2044 8211 947 5152 6070 3466 924 4053 9095 6966 6530 6364 8921 922 5206 9210 7637 9691 1533 7587 9293 5248 4280 5813 8063 288 4879 7440 1571 333 5259 5368 5190 1446 447 9926 1693 8687 8751 5690 2918 4062 1348 6896 6435 1250 6976 9752 3300 8080 5602 5728 3636 4806 9436 2081 4718 5991 3792 5739 4263 157 5465 1306 9936 7230 8253 4283 5564 8813 536 4233 4853 2866 1591 7336 9009 1283 4267 9113 212 2165 2907 3882 4875 6582 3104 6643 6212 1316 303 2373 3056 3983 3304 3562 651 8079 632 7563 5954 1109 457 8577 7291 8029 7104 9397 1893 6931 9084 273 4836 9884 3134 7538 5413 751 9607 9982 746 3653 9358 2345 2116 5121 4450 4341 1883 5657 9528 1590 4844 6023 8999 2743 926 886 9898 1293 9075 1736 4685 7640 6474 5243 3533 3132 3460 504 8120 4747 1958 6974 9850 5681 2175 4648 6307 1778 1706 2553 244 9572 5387 1638 7262 2586 4522 5499 4689 9637 193 6231 5925 2053 6449 1913 9200 9685 7272 9031 5234 
```

Предполагаемый вывод:
```
ArrayB: 50979600 31158724 164836 15928081 85803169 2576025 62047129 1466521 68161536 64673764 22781529 72216004 23280625 11390625 69222400 8042896 7075600 4251844 84143929 8673025 21492496 12264004 64673764 56100100 97871449 1602756 11778624 373321 4618201 32126224 88924900 66569281 14784025 92160000 17164449 63457156 1721344 89908324 47775744 83795716 5290000 1010025 2979076 93489561 33849124 4318084 30924721 19571776 277729 44756100 28451556 2208196 49575681 68508729 36012001 3323329 71520849 6395841 97278769 1527696 64883025 24990001 78889924 69839449 66161956 51638596 1716100 59923081 73290721 27730756 398161 86750596 80425024 69655716 17623204 21609 88284816 23707161 95218564 4008004 19784704 182329 35545444 46703556 46922500 20502784 191844 543169 95726656 21446161 6355441 2119936 96786244 52056225 50197225 3606201 49688401 448900 22762441 12089529 3363556 27352900 17673616 37957921 2160900 93915481 12320100 7452900 6901129 67848169 3771364 43086096 6084 20322064 15745024 43970161 71825625 535824 68906601 555025 351649 15132100 3713329 69572281 45265984 39702601 89226916 23648769 1792921 1677025 68475625 32467204 5832225 34225 1210000 17255716 36336784 25452025 16032016 54756 79619929 26666896 25715041 11492100 3798601 15129 35676729 1024144 58798224 53860921 68973025 41357761 88887184 31945104 14341369 30869136 6874884 50310649 85340644 41718681 41679936 96805921 37773316 50452609 31036041 88868329 42941809 66863329 7284601 751689 30902481 32798529 2876416 82283041 66863329 98465929 47375689 30162064 80209936 27878400 59567524 57002500 31416025 34480384 91776400 7387524 14661241 27227524 913936 7579009 71859529 5294601 36820624 61504 3833764 14953689 40640625 40246336 25120144 20115225 31102929 58186384 83740801 531441 64400625 4613904 11048976 133956 9012004 94672900 97732996 774400 37920964 2380849 99900025 295936 17147881 13764100 9572836 917764 58798224 4844401 69355584 9665881 9610000 60403984 42849 93392896 790321 44009956 84732025 797449 182329 86806489 16711744 14884 3027600 69689104 276676 9622404 36156169 14348944 51667344 61449921 1679616 14707225 49126081 11840481 12830724 7096896 66863329 63536841 1301881 108900 80712256 26853124 30647296 36772096 47114496 69672409 33085504 50523664 5484964 263169 68260644 30869136 19245769 73839649 49984900 3526884 58522500 61748164 20548089 21058921 3598609 864900 48734361 64593369 34609689 30063289 5331481 3045025 78978769 9796900 8048569 75933796 25816561 54730404 94303521 64513024 72965764 29833444 78960996 33825856 608400 24403600 1223236 31979025 21511044 30349081 148996 57108249 24631369 488601 32867289 603729 32524209 381924 11215801 17901361 72046144 2149156 34692100 47734281 12327121 73942801 59136100 4177936 67420521 896809 26543104 36844900 12013156 853776 16426809 82719025 48525156 42640900 40500496 79584241 850084 27102436 84824100 58323769 93915481 2350089 57562569 86359849 27541504 18318400 33790969 65011969 82944 23804641 55353600 2468041 110889 27657081 28815424 26936100 2090916 199809 98525476 2866249 75463969 76580001 32376100 8514724 16499844 1817104 47554816 41409225 1562500 48664576 95101504 10890000 65286400 31382404 32809984 13220496 23097636 89038096 4330561 22259524 35892081 14379264 32936121 18173169 24649 29866225 1705636 98724096 52272900 68112009 18344089 30958096 77668969 287296 17918289 23551609 8213956 2531281 53816896 81162081 1646089 18207289 83046769 44944 4687225 8450649 15069924 23765625 43322724 9634816 44129449 38588944 1731856 91809 5631129 9339136 15864289 10916416 12687844 423801 65270241 399424 57198969 35450116 1229881 208849 73564929 53158681 64464841 50466816 88303609 3583449 48038761 82519056 74529 23386896 97693456 9821956 56821444 29300569 564001 92294449 99640324 556516 13344409 87572164 5499025 4477456 26224641 19802500 18844281 3545689 32001649 90782784 2528100 23464336 36276529 80982001 7524049 857476 784996 97970404 1671849 82355625 3013696 21949225 58369600 41912676 27489049 12482089 9809424 11971600 254016 65934400 22534009 3833764 48636676 97022500 32273761 4730625 21603904 39778249 3161284 2910436 6517809 59536 91623184 29019769 2683044 52736644 6687396 20448484 30239001 21986721 92871769 37249 38825361 35105625 4214809 41589601 3659569 84640000 93799225 52881984 81558961 27394756
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test9C.png)

---
10) Ввод: 
```
1000
3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 
```

Предполагаемый вывод:
```
ArrayB: 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 9 
```

Вывод программы на optimized.s:

![](https://github.com/kolpakovee/avs_idz1/blob/main/tests/test10C.png)

---
![6_4](https://github.com/kolpakovee/avs_idz1/blob/main/criteria/6_4.png)
- Информация добавлена в отчёт.
