# module_5_2

class House:
    def __init__(self,name, number_of_floors):
        self.name = name
        self.number = number_of_floors
    def go_to(self, new_floor):
        if int(new_floor) < 1 or int(new_floor) > int(self.number):
            print("Такого этажа не существует")
        else:
            i = 1
            while i <= int(new_floor):
                print(i)
                i += 1
    def __len__(self):
        return self.number
    def __str__(self):
        return f"Название: {self.name}, кол-во этажей: {self.number}"
h1 = House('ЖК Горский', 18)
h2 = House('Домик в деревне', 2)
print(h1)
print(h2)
print(len(h1))
print(len(h2))
