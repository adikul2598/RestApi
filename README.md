## Class , Loop, FUNCTION

    class Store:

    def __init__(self, name):

        self.name=name

        self.items=[]

    def add_item(self, name, price):

      dict={'name':name,'price':price}

      self.items.append(dict)

    def stock_price(self):

      total=0

    for item in self.items:

        total+=item['price']

        return total
      
## Static & Method

     class Store:

     def init(self, name):

     self.name = name

     self.items = []
    def add_item(self, name, price):

     self.items.append({

     'name': name,

     'price': price
        })
    def stock_price(self):

      total = 0

      for item in self.items:

      total += item['price']

      return total
    @classmethod

     def franchise(cls, store):

         return cls(store.name+" - franchise")
    @staticmethod

     def store_details(store):

        return '{}, total stock price:{}'.format(store.name, int(store.stock_price()))
