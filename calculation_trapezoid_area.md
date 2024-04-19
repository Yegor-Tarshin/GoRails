# Calculation of trapezoid area

```
puts("Good morning, my dear students!")
puts("Today i'll give you a secret knowledge - how to calculate a trapezoid area!")

def calculate_trapezoid_area()
  print("Enter a: ")
  a = gets().chomp().to_i()

  print("Enter b: ")
  b = gets().chomp().to_i()

  print("Enter h: ")
  h = gets().chomp().to_i()

  s = ((a + b) / 2) * h

  puts("When a = #{a}, b = #{b}, h = #{h}: The square is #{s}")
end

calculate_trapezoid_area()
calculate_trapezoid_area()
calculate_trapezoid_area()
```
