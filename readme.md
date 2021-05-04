Одна статья на хабре вынудила меня сделать эти бенчмарки. В ней сравнивалась наивная рекурсия и замыкания, это было странновато и мне самому захотелось все проверить добавив пару новых вариантов.

Примерные результаты:

Наивная рекурсия (rec.py)        - 5.85 ms            
Замыкания (closure.py)           - 2.30 ms              
Хвостовая рекурсия (tail_rec.py) - 2.71 ms              
Мемоизация (memo.py)             - 1.78 ms

В итоге получается что хвостовая рекурсия почти не уступает по скорости методу автора статьи и при этом обладает большей лаконичностью, а мемоизация проще и быстрее всех остальных вариантов, при этом лишь ненамного уступая в простоте наивной рекурсии, чьей модификацией собственно и является

----------

One article on Habr[https://habr.com/ru/all/] made me do these benchmarks. Its author compared naive recursion and closures, it was strange, and I wanted to check everything myself, adding a couple of new options.
