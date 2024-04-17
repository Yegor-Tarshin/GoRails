# Five little monkeys song
## Task
Write a song

Five little monkeys jumping on the bed,
One fell off and bumped his head.
Mama called the doctor and the doctor said,
"No more monkeys jumping on the bed!"

Four little monkeys jumping on the bed,
One fell off and bumped his head.
Mama called the doctor and the doctor said,
"No more monkeys jumping on the bed!"

Three little monkeys jumping on the bed,
One fell off and bumped his head.
Mama called the doctor and the doctor said,
"No more monkeys jumping on the bed!"

Two little monkeys jumping on the bed,
One fell off and bumped his head.
Mama called the doctor and the doctor said,
"No more monkeys jumping on the bed!"

One little monkey jumping on the bed,
He fell off and bumped his head.
Mama called the doctor and the doctor said,
"Put those monkeys straight to bed!"

```
index = 5

while (index > 0)
  if index > 1
    puts("#{index} little monkeys jumping on the bed,")
  else
    puts("1 little monkey jumping on the bed,")
  end

  if index > 1
    puts("One fell off and bumped his head.")
  else
    puts("He fell off and bumped his head.")
  end

  puts("Mama called the doctor and the doctor said,")

  if index > 1
    puts("No more monkeys jumping on the bed!")
  else
    puts("Put those monkeys straight to bed!")
  end

  index = index - 1

  puts()
end
```
## Comments

Цикличная песня, где в первых четыре куплета повторяются за исключением 1-го слова.
Последний куплет - повторяется только 3 строка.

index = 5 (задаём цикл, где 5 означает, с какого числа начинать цикл)

while (index > 0) (показывает до какого момента выполняется цикл)

if index > 1
    puts("#{index} little monkeys jumping on the bed,")
 пока индекс больше 1 - puts("#{index} little monkeys jumping on the bed,") 
 
 else
    puts("Put those monkeys straight to bed!")
 если условие if index > 1, вставить следующее значение.
 
 end
```
