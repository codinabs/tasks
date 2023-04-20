#Задание 1

import re 
result = re.search(r'Alabama','Sweet home Alabama')
print(result.group(0))

#Задание 2

import re 
result = re.sub(r'Alabama','Omaha','Sweet home Alabama')
print(result)

#Задание 3

import re 
result = re.findall(r'Bulka','Bulka s makom and Bulka s koritsey')
print(result)

#Задание 4

import re
result = re.match(r'Mr','Mr boombastic')
print(result.group(0))

#Задание 5

import re
result = re.split(r'a','Sweet home Alabama', maxsplit = 2) 
print(result)

#Задание 6

import re
result = re.findall(r'snow/*','let it snow let it snow')
print(result)

#Задание 7

import re
result = re.findall(r'\d{1}','123 1 22 33 2')
print(result)

#Задание 8

import re
result = re.findall(r'^\w+','Sweet home Alabama')
result1 = re.findall(r'\w+$','Sweet home Alabama')
print(result,result1)

#Задание 9

import re
result = re.findall(r'Sweet|Alabama','Sweet home Alabama')
print(result)

#Задание 10 

import re
result = r.findall(r'([a-z]+)(\d*)','one1, two2, three3, four4')
print(result)

#Задание 12

import re

s = input()
kk = re.findall(r'(?<=[QWRTYPSDFGHJKLZXCVBNMqwrtypsdfghjklzxcvbnm])[aeuioAEUIO]{2,}(?=[QWRTYPSDFGHJKLZXCVBNMqwrtypsdfghjklzxcvbnm])', s)

if len(kk) > 0:
  for element in kk:
    print(element)
else:
  print(-1)
