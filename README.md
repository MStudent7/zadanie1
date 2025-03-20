# zadanie1
Repozytorium do Zadania nr 1

Opis programu:
Program zawiera funkcje takie jak:
Funkcja zip() tworzy obiekt, który łączy elementy dwóch lub więcej list.
Funkcja sqrt() oblicza pierwiastek z podanej liczby.
Obsługa wyjątki ValueError, przykładowo dla programu gdy dane nie są liczbą, a musimy obliczyc pierwiastek.

  import math
  
  imie = ["Karol", "Emilia", "Aleksandra"]
  punkty = [79, 85, 95]
  
  # Łączenie dwóch list za pomocą funkcji zip().
  # Funkcja zip() tworzy obiekt, który łączy elementy dwóch lub więcej list w krotki.
  # Link do dokumentacji: https://docs.python.org/3/library/functions.html#zip
  laczenie = zip(imie, punkty)
  
  print("Lista laczona - zip():")
  for imie, punkty in laczenie:
      print(f"{imie}: {punkty}")
  
  # Wykorzystanie sqrt() z math.
  # Funkcja sqrt() oblicza pierwiastek z podanej liczby.
  # Link do dokumentacji: https://docs.python.org/3/library/math.html#math.sqrt
  liczba = 16
  print("\nPierwiastek:", math.sqrt(liczba))
  
  try:
      user_input = input("\nWprowadź liczbę, aby obliczyć pierwiastek: ")
      num = float(user_input) 
      print("Pierwiastek to:", math.sqrt(num))
  except ValueError:
      # Obsługa wyjątku ValueError, gdy dane nie są liczbą.
      # Link do dokumentacji: https://docs.python.org/3/library/exceptions.html#ValueError
      print("Wprowadzona wartość to nie liczba!")
