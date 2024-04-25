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
2. 
Please, enter your TODO text:

<ENTERING OUR TEXT...>
  
Your TODO

<ENTERED TEXT...>
  
Has been successfully added.

4. Update TODO

Please, enter index of TODO you want to modify

<ENTERING OUR NUMBER...>
  
(@TODO Add index existance check)

Please, enter new text for this TODO

<ENTERING OUR NEW TEXT...>
  
TODO at index <INDEX> has been successfully modified to:

<NEW ENTERED TEXT...>


5. Delete TODO
Please, enter index of TODO you want to delete
(@TODO Add index existance check)
TODO at index <INDEX> has been successfully deleted.

## Code
```
TODO_list = []

puts("MENU OPTIONS")
puts("1. Create TODO")
puts("2. Read TODOs")
puts("3. Update TODO")
puts("4. Delete TODO")
puts("0. Exit")


begin
  print("Choose your option: ")
  text = gets().chomp().to_i()

  if (text == 1)
    print("Please, enter your TODO text: ")
    text = gets().chomp()
    TODO_list.push(text)
    puts("Your #{text} has been successfully added")

  elsif (text == 2)
    puts("#{TODO_list}")

  elsif (text == 3)
    print("Please, enter index of TODO you want to modify: ")
    index = gets().chomp().to_i()
    print("Please, enter new text: ")
    TODO_list[index] = gets().chomp()
    puts("TODO at index #{index} has been successfully modified to #{TODO_list[index]}")

  elsif (text == 4)
    print("Please, enter index of TODO you want to delete: ")
    index = gets().chomp().to_i()
    TODO_list.delete_at(index)
    puts("TODO index #{index} has been successfully deleted!")

  elsif (text == 0)
    break
  end
end while(text.size)

```
