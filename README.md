# HW2_hash_practice
inputfile=open('hw2_data.txt','r')
foods=[]
for i in inputfile:
    i=i.replace('\n','')
    foods.append(i)
food_count = {}

for food in foods:
    if food in food_count:
        food_count[food] += 1
    else:
        food_count[food] = 1

print("共有"+str(len(food_count))+"個不重複的英文字")
for food, count in food_count.items():
    print(f"{food}: {count}次")

#Results
共有10個不重複的英文字
Cheese: 234次
Pizza: 83次
Coke: 145次
Steak: 46次
Burger: 196次
Fries: 76次
Rib: 33次
Taco: 57次
Pho: 19次
Potato: 3次
