```python
fahrenheit_val = 99
celsius_val = ((fahrenheit_val - 32) *(5/9))

print(celsius_val)
```

    37.22222222222222



```python
fahrenheit_val2 = 43
celsius_val2 = ((fahrenheit_val2 - 32) * (5/9))

print(celsius_val2)
```

    6.111111111111112



```python
def explicit_fahr_to_celsius(temp):
    # Assign the converted value to a variabel
    converted = ((temp - 32) * (5/9))
    # Return the values of the new variable
    return converted
```


```python
def fahr_to_celsius(temp):
    # Return converted values more efficietntly using the return function without creating 
    # a neww variable. This code does not mean the same thing as the previous function but it is more 
    # explicit in explaining how the command works
    return ((temp - 32) * (5/9))
```


```python
fahr_to_celsius(32)
```




    0.0




```python
explicit_fahr_to_celsius(32)
```




    0.0




```python
print('Freezing point of water:', fahr_to_celsius(32), 'C')
print('Boiling point of water:', fahr_to_celsius(212), 'C')
```

    Freezing point of water: 0.0 C
    Boiling point of water: 100.0 C



```python
def celsius_to_kelvin(temp_c):
    return temp_c + 273.15

print('freezing point of water in kelvin:', celsius_to_kelvin(0.))
```

    freezing point of water in kelvin: 273.15



```python
def fahr_to_kelvin(temp_f):
    temp_c = fahr_to_celsius(temp_f)
    temp_k = celsius_to_kelvin(temp_c)
    return temp_k

print('freezing point of water in Kelvin:', fahr_to_kelvin(212.0))
```

    freezing point of water in Kelvin: 373.15



```python
print('Again, temperature in kelvin was:', temp_k)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    <ipython-input-19-4e4efe6231e3> in <module>
    ----> 1 print('Again, temperature in kelvin was:', temp_k)
    

    NameError: name 'temp_k' is not defined



```python
temp_kelvin = fahr_to_kelvin(212.0)
print('Temperature in Kelvin was:', temp_kelvin)
```

    Temperature in Kelvin was: 373.15



```python
def print_temperatures():
    print('Temperature in fahrenheit was:', temp_fahr)
    print('Temperature in kelvin was:', temp_kelvin)
    
    temp_fahr = 212.0
    temp_kelvin = fahr_to_kelvin(temp_fahr)
    
    print_temperatures()
```


```python
def print_temperatures():
    print('Temperature in farenheit was:', temp_fahr)
    print('Temperature in kelvin was:', temp_kelvin)
    
temp_fahr = 212.0
temp_kelvin = fahr_to_kelvin(temp_fahr)

print_temperatures()
```

    Temperature in farenheit was: 212.0
    Temperature in kelvin was: 373.15



```python

```
