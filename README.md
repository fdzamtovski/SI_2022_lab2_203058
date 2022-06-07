# Втора лабораториска вежба по Софтверско инженерство
## Филип Џамтовски, бр. на индекс 203058
## Control Flow Graph
Фотографија од control flow graph-ot:
![Graph](https://user-images.githubusercontent.com/76556606/171952528-3ff0ab57-f398-4d43-a29c-588aa8b62f82.png)

## Цикломатска комплексност
M = E – N + 2P
E - број на edges во CFG
N - број на nodes во CFG
P - број на поврзани компоненти

E = 28
N = 23
P = 1

M = 28 - 23 + 2 * 1
M = 7

## Тест случаи според критериумот Every statement
![image](https://user-images.githubusercontent.com/76556606/172363396-643f5b33-7500-447a-b312-d2e25a67a848.png)

## Тест случаи според критериумот Every path
....

## Објаснување на напишаните unit tests
Првиот тест го правам со assertEquals(list, mk.ukim.finki.SILab2.function(resultList)) каде проверувам дали list е иста со листата вратена после функцијата function(resultList).

Вториот тест го правам со IllegalArgumentException thrown = Assertions.assertThrows(IllegalArgumentException.class, () -> mk.ukim.finki.SILab2.function(exceptionList)), каде креирам исклучок од класата IllegalArgumentException. Кога ќе се изврши function() треба да ја врати пораката од exception. Вака проверувам дали е вратена порака од соодветниот исклучок assertEquals("List length should be greater than 0", thrown.getMessage());

Третиот тест го правам со IllegalArgumentException thrown2 = Assertions.assertThrows(IllegalArgumentException.class, () -> mk.ukim.finki.SILab2.function(exceptionList2)), каде креирам исклучок од класата IllegalArgumentException. Кога ќе се изврши function() треба да ја врати пораката од exception. Вака проверувам дали е вратена порака од соодветниот исклучок assertEquals("List length should be a perfect square", thrown2.getMessage());
