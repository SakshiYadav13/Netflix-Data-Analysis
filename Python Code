import pandas as pd

import sqlalchemy as sal

df = pd.read_csv('netflix_titles.csv')

engine = sal.create_engine('mssql://LAPTOP-57QR538I\SQLEXPRESS/master?driver=ODBC+DRIVER+17+FOR+SQL+SERVER')
conn= engine.connect()

df.to_sql('netflix', con = conn, index = False, if_exists = 'append')
conn.close()

len(df)

df[df.show_id == 's5023']

max(df.show_id.dropna().str.len())

max(df.type.dropna().str.len())

max(df.title.dropna().str.len())

max(df.director.dropna().str.len())

max(df.cast.dropna().str.len())

max(df.country.dropna().str.len())

max(df.date_added.dropna().str.len())

max(df.release_year.dropna().str.len())

max(df.rating.dropna().str.len())

max(df.duration.dropna().str.len())

max(df.listed_in.dropna().str.len())

max(df.description.dropna().str.len())


df.isna().sum()
