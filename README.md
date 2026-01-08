def celcius_to_fahrenheit(celcius):
    return (celcius * 9/5) + 32

def fahrenheit_to_celcius(fahrenheit):
    return (fahrenheit - 32) * 5/9

def kelvin_to_celcius(kelvin):
    return kelvin - 273.15

print("Wähle eine Einheit für die Umrechnung")
print("(1) Celsius nach Fahrenheit")
print("(2) Fahrenheit nach Celsius")
print("(3) Kelvin nach Celsius")
wahl = int(input("Deine Wahl: "))

if wahl == 1:
   celsius = float(input("Gib die Temperatur in Celsius ein: "))
   fahrenheit = celcius_to_fahrenheit(celsius)
   print(f"{celsius} Celsius sind {fahrenheit} Fahrenheit")

elif wahl == 2:
   fahrenheit = float(input("Gib die Temperatur in Fahrenheit ein: "))
   celsius = fahrenheit_to_celcius(fahrenheit)
   print(f"{fahrenheit} Fahrenheit sind {celsius} Celsius")

elif wahl == 3:
   kelvin = float(input("Gib die Temperatur in Kelvin ein: "))
   celsius = kelvin_to_celcius(kelvin)
   print(f"{kelvin} Kelvin sind {celsius} Celsius")

else:
   print("Ungültige Wahl")
   
