puts("Welcome to Finance App!")

puts()

puts("Menu options")
puts("1. Create entry")
puts("2. Read entries")
puts("3. Update entry")
puts("4. Delete entry")
puts("5. Get total price. (Please, buy PREMIUM EDITION)")

entries = [{"title" => "Milk", "price" => 10, "amount" => 5}, {"title" => "Fish", "price" => 8, "amount" => 17}]

puts()

while (true)
  print("Choose your option: ")
  option = gets().chomp().to_i()
  entry = {"title"=> nil, "price"=> nil, "amount"=> nil}

  if (option == 1)
    print("Please, enter product title: ")
    entry["title"] = gets().chomp()
    print("Please, enter a price: ")
    entry["price"] = gets().chomp().to_i()
    print("Please, enter number of items: ")
    entry["amount"] = gets().chomp().to_i()

    entries.push(entry)

    puts()

    puts("#{entry["title"]} with the price of #{entry["price"]} in amount of #{entry["amount"]} has been added to your list.")

  elsif (option == 2)
    puts("#{entries}")

  elsif (option == 3)
    print("Enter index of product you want to update: ")
    index = gets().chomp().to_i()
    puts("You have chosen #{entries[index]}")
    print("What do you want to change?
      1. Title
      2. Price
      3. Amount
      4. Increment amount
      enter your choice: ")
    choice = gets().chomp().to_i()
    if (choice == 1)
      print("Enter a new title: ")
      entries[index]["title"] = gets().chomp()
      puts("#{entries}")
    elsif (choice == 2)
      print("Enter a new price: ")
      entries[index]["price"] = gets().chomp().to_i()
      puts("#{entries}")
    elsif (choice == 3)
      print("Enter a new amount: ")
      entries[index]["amount"] = gets().chomp().to_i()
      puts("#{entries}")
    elsif (choice == 4)
      entries[index]["amount"] = entries[index]["amount"] + 1
      puts("#{entries}")
    end

  elsif (option == 4)
    print("Enter index of product you want to delete: ")
    index = gets().chomp().to_i()
    buffer = entries[index]
    entries.delete_at(index)
    puts("#{buffer} has been successfully deleted.")

  elsif (option == 5)
    index = 0
    sum = 0
    while(index < entries.size())
      sum = sum + entries[index]["price"] * entries[index]["amount"]
      index = index + 1
    end

    puts("Your total sum is: #{sum}")

  end


end
