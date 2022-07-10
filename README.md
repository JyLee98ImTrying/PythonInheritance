# PythonInheritance
How to code inheritance thingys in python


#Fruity Inheritance 
class Fruit: 
    def __init__(self, color, flavor):
        self.color = color
        self.flavor = flavor

class Apple(Fruit):
    pass

class Grape(Fruit):
    pass 

granny_smith = Apple("green" , "crunchy")
eygption = Grape ("purple","squishy")
print(granny_smith.flavor)

pass 



#Clothing Inheritance

class Clothing:
  material = ""
  def __init__(self,name):
    self.name = name
  def checkmaterial(self):
	  print("This {} is made of {}".format(self.name,self.material))
			
class Shirt(Clothing):
  material="Cotton"

polo = Shirt("Polo")
polo.checkmaterial()


# Piggy Inheritance


class Animal:
     sound = ""
     def __init__(self, name):
         self.name = name
     def speak(self):
         print("{sound} I'm {name}! {sound}".format(
             name=self.name, sound=self.sound))
 
class Piglet(Animal):
     sound = "Oink!"
 
class Cow(Animal):
     sound = "Moooo"
     
hamlet = Piglet("Hamlet")
hamlet.speak()
