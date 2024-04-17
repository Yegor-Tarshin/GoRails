# Rest of you life program

```
puts('Hello!')
puts('Here you can get how many years left in your life')

def calculate_rest_of_life()

  print('Enter you age: ')

  current = gets().chomp().to_i()

  rest = 100 - current

  puts("The rest of your life is #{rest}")

end


calculate_rest_of_life()
```

## Usage example 

```
Hello!

Here you can get how many years left in your life

Enter you age: 43

The rest of your life is 57
```
