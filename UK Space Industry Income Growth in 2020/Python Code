#IMPORT DATA

#UK Space Industry Income Growth in 2020/21 by Sector

import pandas as pd
import plotly.express as px
import csv
with open('Space Data.CSV', 'r') as csv_file:
    csv_reader = csv.DictReader(csv_file)

df=pd.read_csv('Space Data.CSV')

#FINDING MAX

#print("The highest area of growth in the UK Space is", x, "at", p "%")

s = df.loc[df["Growth"].idxmax()]

print("The industry with the highest growth is",f"{s.Name} at:\t{s.Growth}%")
#piechart

fig = px.pie(df, values='Growth', names='Name', title='UK Space Industry Income Growth in 2020/21 by Sector ')
fig.show()
