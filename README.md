Требуется разработать на языке JavaScript код, печатающий на консоль самую длинную общую подстроку всех переданных строк. Строки передаются параметрами командной строки в ваш JavaScript, выполняемый под Node.js. Если самая длинная общая подстрока является пустой строкой (например, не было передано ни одной строки или строки не имеют общих для всех символов), напечатать один перевод строки (пустую строку). При существовании нескольких решений — напечатать одно решение (любое). Вывод всегда сопровождается переводом строки. Ограничения: длина одной строки не превосходит 256 символов, количество строк не превосходит 64, строки содержат только латинские буквы и арабские цифры, время выполнения одного теста - не более пяти секунд, вывод не содержит посторонних символов. Ограничения не должны быть в вашем коде, это ограничения на автоматические тесты.

Решение будет приниматься при прохождении набора тестов, результат будет оцениваться исходя из размера файла в байтах (меньше — лучше). Соответственно, никаких комментариев, длинных имён, отступов и прочего.

Файл должен иметь имя lcs.js (вот именно такое). Обязательно использование параметров командной строки (никаких readline, process.stdin и т.п.; ТОЛЬКО process.argv).

Пример:

node lcs.js ABCDEFZ WBCDXYZ

BCD

Несколько возможных тестов (в случае существования нескольких решений вывод может отличаться в соответствии с условием задачи):

node lcs.js 132 12332 12312

1

node lcs.js ABCDEFGH ABCDEFG ABCEDF ABCED

ABC

node lcs.js ABCDEFGH ABCDEFG ABCEDF ABCED

ABC

node lcs.js ABCDEFGH ABCDEFG ABCDEF ABCDE

ABCDE

node lcs.js ABCDEFGH ABCDEFG ABCDEF ABCDE EDCBA

A

node lcs.js ABCDEFGH ABCDEFG ABCDEF ABCDE EDCBCA

BC

node lcs.js ABCDEFGH ABCDEFG AxBCDEF ABCDxE EDCBCAABCD

BCD

node lcs.js ABCDEFGH 1234

node lcs.js ABCDEFGH

ABCDEFGH