# Error: Parse error on line 4:
# ...ите 2-ю цифру: d2 = (N // 100) % 10]   
# -----------------------^
# Expecting 'SEMI', 'NEWLINE', 'SPACE', 'EOF', 'GRAPH', 'DIR', 'subgraph', 'SQS', 'SQE', 'end', 'AMP', 'DOUBLECIRCLEEND', 'PE', '-)', 'STADIUMEND', 'SUBROUTINEEND', 'ALPHA', 'COLON', 'PIPE', 'CYLINDEREND', 'DIAMOND_STOP', 'TAGEND', 'TRAPEND', 'INVTRAPEND', 'START_LINK', 'LINK', 'STYLE', 'LINKSTYLE', 'CLASSDEF', 'CLASS', 'CLICK', 'DOWN', 'UP', 'DEFAULT', 'NUM', 'COMMA', 'MINUS', 'BRKT', 'DOT', 'PCT', 'TAGSTART', 'PUNCTUATION', 'UNICODE_TEXT', 'PLUS', 'EQUALS', 'MULT', 'UNDERSCORE', got 'PS'
graph TD;
    A[Начало] --> B[Введите четырехзначное число N]
    B --> C[Извлеките 1-ю цифру: d1 = N // 1000]
    C --> D[Извлеките 2-ю цифру: d2 = (N // 100) % 10]
    D --> E[Извлеките 3-ю цифру: d3 = (N // 10) % 10]
    E --> F[Извлеките 4-ю цифру: d4 = N % 10]
    F --> G[Посчитайте сумму первых двух: Sum1 = d1 + d2]
    G --> H[Посчитайте сумму последних двух: Sum2 = d3 + d4]
    H --> I{Sum1 == Sum2?}
    I --> |Да| J[Выведите "Суммы равны"]
    I --> |Нет| K[Выведите "Суммы не равны"]
    J --> L[Конец]
    K --> L
