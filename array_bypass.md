# Array bypass (Обход массива)

```
a = [2, 5, 58, 84, 32, 50, 0, 43, 49, 65, 99]

index = 0
size = a.size()

while(index < a.size() )
  puts("Элемент массива \"a\" под порядковым номером #{index} = #{a[index]}")
  index = index + 1
  puts()
end
```

Элемент массива "a" под порядковым номером 0 = 2

Элемент массива "a" под порядковым номером 1 = 5

Элемент массива "a" под порядковым номером 2 = 58

Элемент массива "a" под порядковым номером 3 = 84

Элемент массива "a" под порядковым номером 4 = 32

Элемент массива "a" под порядковым номером 5 = 50

Элемент массива "a" под порядковым номером 6 = 0

Элемент массива "a" под порядковым номером 7 = 43

Элемент массива "a" под порядковым номером 8 = 49

Элемент массива "a" под порядковым номером 9 = 65

Элемент массива "a" под порядковым номером 10 = 99

## Comments
index = 0  - указывается для того, чтобы отсчёт вёлся с 1-го элемента массива

size = a.size() - указывает, что размер - это размер массива А

while(index < a.size() ) - указывает, что цикл продолжается до тех пор пока индекс по формуле index = index +1 не превысит количество элементов массива, так как a.size - это число следующее за последним элементом массива.
puts("Элемент массива \"a\" под порядковым номером #{index} = #{a[index]}")

\"a\" чтобы кавычки не считывались оператором, мы закрываем их обратным слешом

#{index} - интерполяция index = index +1 в ходе выполнения цикла

#{a[index]} - интерполяция index = index +1 из массива А в ходе выполнения цикла

index = index + 1 (Цикл начинается с вычисления index = 0 +1, так как в начале мы задали, что индекс равен нулю. В ходе следующего вычисления index = 1 +1. В ходе следующего index = 2 +1 и так далее.

puts() - ставит пробелы между циклами.
