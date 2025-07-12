# python35
Greet values
def titled(title):
    def greet(name):
        return f"Hello,{title}{name}"
    return greet
mr_greet=titled("Mr.")
dr_greet=titled("Dr.")
print(mr_greet("Siddu"))
print(dr_greet("Sweetie"))

Globally & Locally values
x=100
y=10
def display():
    x=22
    print("x=",x)
    print("locally",x+y)
display()
print("x=",x)
y=10
y=25
print("latest value of globally",x+y)
