# TODO program

## Task
Create TODO program

Menu:
1. Create TODO
2. Read TODOs
3. Update TODO
4. Delete TODO
0. Exit

[]

["Cook food", "Train in the morning"]

2. Read TODOs

0. Cook food
1. Train in the morning
...

1. Create TODO
Please, enter your TODO text:
<ENTERING OUR TEXT...>
Your TODO
<ENTERED TEXT...>
Has been successfully added.

3. Update TODO
Please, enter index of TODO you want to modify
<ENTERING OUR NUMBER...>
(@TODO Add index existance check)
Please, enter new text for this TODO
<ENTERING OUR NEW TEXT...>
TODO at index <INDEX> has been successfully modified to:
<NEW ENTERED TEXT...>

4. Delete TODO
Please, enter index of TODO you want to delete
(@TODO Add index existance check)
TODO at index <INDEX> has been successfully deleted.

## Code
```
a = []

puts("
MENU OPTIONS
1. Create TODO
2. Read TODOs
3. Update TODO
4. Delete TODO
0. Exit")



begin
  print("Choose your option: ")
  text = gets().chomp().to_i()

  if (text == 1)
    print("Please, enter your TODO text: ")
        a.push(gets().chomp())
    puts("Your #{a.push} has been successfully added")

  elsif (text == 2)
    puts("#{a}")

  elsif (text == 3)
    print("Please, enter index of TODO you want to modify: ")
    i = gets().chomp().to_i()
    print("Please, enter new text: ")
      a[i] = gets().chomp()
    puts("TODO at index #{i} has been successfully modified to #{a[i]}")

  elsif (text == 4)
    print("Please, enter index of TODO you want to delete: ")
    i = gets().chomp().to_i()
    a.delete_at(i)
    puts("TODO index #{i} has been successfully deleted!")

  elsif (text == 0)
    break
  end
end while(text.size)

```
