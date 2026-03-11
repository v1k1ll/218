# №2 ЕГЭ информатика
## №18614 https://inf-ege.sdamgia.ru/problem?id=18614


# Задание 8 из ЕГЭ по информатике
## №27539 [https://inf-ege.sdamgia.ru/problem?id=17328](https://inf-ege.sdamgia.ru/problem?id=27539)
## <img width="835" height="49" alt="image" src="https://github.com/user-attachments/assets/f636e718-1be8-4bf6-b7e1-a94b51e50730" />

```
import itertools
alphabet = "БОРИС"
ar = itertools.product(alphabet, repeat=6) #Размещение с повторением
arl = []
for i in ar:
    arl.append(list(i))
count = 0
for e in arl:
    if e.count("Б") == 1 and e.count("Р") == 1 and e.count("С") <= 1:
        count += 1
print(count)
```
### Ответ: 1440

## №28685 [[https://inf-ege.sdamgia.ru/problem?id=17328](https://inf-ege.sdamgia.ru/problem?id=18079)](https://inf-ege.sdamgia.ru/problem?id=28685)
## <img width="830" height="43" alt="image" src="https://github.com/user-attachments/assets/9cf15df0-2e88-4df2-949b-e09ed3d23274" />

```
from itertools import product
count = 0
for x in product('ПЕТЯ', repeat=6):
    slovo = ''.join(x)
    if all(pair not in slovo for pair in 'ПП ПТ ТП ТТ ЕЯ ЯЕ ЕЕ ЯЯ'.split()):
        count += 1
print(count)
```
### Ответ: 128

## №7306 [[inf-ege.sdamgia.ru/problem?id=18491](https://inf-ege.sdamgia.ru/problem?id=18491)](https://inf-ege.sdamgia.ru/problem?id=7306)
## <img width="831" height="34" alt="image" src="https://github.com/user-attachments/assets/daa3dfdb-3f1d-4b56-882d-fe1a023b50ce" />

```
begin
'УЧЕНИК'.Cartesian(5)
.Count(s-> s.StartsWith('У')and s.EndsWith('К') )
.Print;//216
end.
```
### Ответ: 216
