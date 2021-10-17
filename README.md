# Product
A class has been created in which name,amount and price of an item is entered by user and in response, output is generated.
class Product:
  def __init__(self,name,amount,price):
    self.name = name
    self.amount = amount
    self.price = price
  def get_price(self):
    if self.amount<10:
      return self.price*self.amount
    elif self.amount>=10 and self.amount<=100:
      return self.price*self.amount*0.9
    elif self.amount>100:
      return self.price*self.amount*0.8
  def make_purchase(self):
    return self.name
    return self.amount
x = Product('Bajaj',101,100)
print(x.make_purchase())
print(x.get_price())
