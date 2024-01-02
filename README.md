#簡易計算器：創建一個程序，允許用戶輸入兩個數字，然後選擇要進行的運算（如加、減、乘、除）。
def add (x,y):
	return x + y
def sub (x,y):
	return x - y
def mul (x,y):
	return x * y
def div (x,y):
	if y == 0:  #除法特別加上除以零錯誤的處理
		return "Error: Cannot divide by zero."
	return x / y
x = int(input("num1:"))
y = int(input("num2:"))
cal = input("choose operation type(+,-,*,/)=")
if cal == "+": #在非計算中用到運算符記得要用“”來把他轉成字符，避免成程式讀取錯誤
	print (f"result={add(x,y)}")
elif cal == "-":
	print (f"result={sub(x,y)}")
elif cal == "*":
	print (f"result={mul(x,y)}")
elif cal == "/":
	print (f"result={div(x,y)}")
else:
	print("error: Invalid operation.")
