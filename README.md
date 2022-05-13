# Diplom
import os
import re
import sqlite3
import csv
import pandas as pd
import os.path


path = 'C:\Python\old'
def getFile(path):
    return os.listdir(path)



file = getFile(path)


for i in file:
    with open(path+ '\\' + i, 'r') as p:
        f = p.readline()
        
        









# filenum = 0
# alllists={''}
# path = 'C:\Python\old'
# for lists in os.listdir(path):
#     sub_path = os.path.join(path, lists)
#     if os.path.isfile(sub_path):
#         filenum = filenum+1
#         alllists.add(lists)
#     elif os.path.isdir(sub_path):
#         dirnum = dirnum+1
        
# print('filenum: ',filenum)





# for file in os.listdir("C:\Python\old"):
#     with open(os.path.join("C:\Python\old", file), 'r') as p:
#         lines = p.readlines()
#         st = lines[0]
#         A = st.split(' ')
# #         print (alllists)
#         for i in alllists:
            
#             print(A[1])
#             print(alllists)
# #             print(i)
#             if (A[1] == alllists ):
# #                 print(A[1])
# #                 print(alllists)
#                 df = pd.DataFrame({
#                     'name': [i],
#                     'size': [A[13]],
#                     'time': [A[5]],
#                     'Lon': [A[6]],
#                     'Lat': [A[7]]
#                     })

#             else: (
#                 print ("error"))
            
            
#             df.to_excel("C:\Python\example.xlsx", )
