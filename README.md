# Diplom
import os
import re
import sqlite3
import csv
import pandas as pd
import os.path

filenum = 0
alllists={''}
path = 'C:\Python\old'
for lists in os.listdir(path):
    sub_path = os.path.join(path, lists)
    if os.path.isfile(sub_path):
        filenum = filenum+1
        alllists.add(lists)
    elif os.path.isdir(sub_path):
        dirnum = dirnum+1
        
print('filenum: ',filenum)


for file in os.listdir("C:\Python\old"):
    with open(os.path.join("C:\Python\old", file), 'r') as p:
        lines = p.readlines()
        st = lines[0]
        A = st.split(' ')
        
        
        
        for i in range(0, len(alllists)):   
            if (A[1] == "SoundVelocity"  ):
                df = pd.DataFrame({
                    'name': [i],
                    'size': [A[13]],
                    'time': [A[5]],
                    'Lon': [A[6]],
                    'Lat': [A[7]]
                    })
            else: (
                print ("error"))
            i=i+1
            
            df.to_excel("C:\Python\example.xlsx", )
