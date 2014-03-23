##Домашна работа 1

## Задачи

Решенията на задачите се предават по e-mail на следните адреси:

* Група 1 - KN13.14.1.1@gmail.com
* Група 2 - kn201317@gmail.com
* Група 3 - lachezarstoev93@gmail.com | ts.kandilarova@gmail.com
* Група 4 - kn4_1314@abv.bg

Срок за предаване: 24.03.2014 - 30.03.2014

Решението на всяка задача трябва да бъде под формата на файлове с окончание *.cpp* и *.h* (не целите проекти, ако използвате Visual Studio). Файловете се изпращат като attachment-и в mail-a. Освен решения на задачите самият mail трябва да съдържа име и факултен номер. Успех!


###Задача-та

    Да се реализира програма, която реализира игра (money steam):
    Играта се играе от двама човека. Създава се масив `money stream`, от цели числа, с дължина n, (n e четно)
    който се запълва със случайни стойности.Двамата хвърлят зар кой ще започне първи.

    Първият избира едно цяло число в range(0, n)
    което ще бъде индекс от масива. Стойноста от клетката на масива е сумата която човека получава. Тази сума се прибавя към общатата му сума с пари. Двата играчи се редуват в избора на индекси докато не останат повече клетки.

    Накрая се извеждат всички избори на двамата човека, и кой е спечелил играта. Печели този с по-голям капитал и се извежда съобщение за повторна игра или за завършване на играта.

    ####За ядрото на играта използвайте следните декларации:
    * Играч се определя от `class Player` със следните атрибути
        * `name` - име на играча с произволна дължина (динамична)
        * `score` - баланс от точки за играча
        * `nickname`
        ----
        * `конструктор` - единствено с параметри
        * `copy-конструктор`
        * `operator=`
        * `get_name`
        * `get_nickname`
        * `get_score`
        * `add_score` - добавя сума към баланса
#####Не са необходими set методи.
    ===
    * Всяка изиграна игра се характеризира с обект от `class MoneyStream` с атрибути:
        * `moneyStream` - масив със случайни числа
        * `size` - големина на масива
        * `players` - играчи (от тип Player)
        ----
        * `конструктор` - единствено с параметри
        * `makeMoneyStream` - взема като параметър цяло число и играч; Ако е възможно, добава сумата от дадената клетка на дадения играч
        * `checkGameStatus` - връща истина ако играта е приключила и предизвиква


###Задача ЕК(бонукс)

    Разширите играта като добавите възможност за игра с бот, който да играе срещу вас(с изкуствен интелект).