# calculator
def add(a, b):
    return a + b 

def sub(a, b):
  return a - b

def mul(a, b):
  return a * b

def div(a, b):
  return a / b

  
print("welcome to the calculator!!!!")
print("Select operation.")
print("1.Add")
print("2.Subtract")
print("3.Multiply")
print("4.Divide")

while True:
  opt = input("Please enter a number from above(1, 2, 3, 4): ")
  if opt in ('1' , '2', '3', '4'):
      a1 = int(input("Enter first number : "))
      b1 = int(input("Enter second number : "))
      
      if opt == '1':
        print(a1, "+", b1, "=", add(a1, b1))
    
      elif opt == '2':
        print(a1, "-", b1, "=", sub(a1, b1))
        
      elif opt == '3':
        print(a1, "*", b1, "=", mul(a1, b1))
      
      elif opt == '4':
        print(a1, "/", b1, "=", div(a1, b1))

      continue_calc = input("want to continue (y/n): ")
      if continue_calc == 'n':
        break
    
  else:
      print("invalid input")
