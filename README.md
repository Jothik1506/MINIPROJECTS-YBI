# Assignment-1
  import pandas as pd

url = "https://github.com/YBIFoundation/Pandas/raw/refs/heads/main/ElectroGadget.csv"
df = pd.read_csv(url)

print(df.head())

df.groupby("Product")["Units Sold"].sum().sort_values(ascending=False)
df.groupby("Category")["Units Sold"].sum().sort_values(ascending=False)


df.groupby("Region")["Revenue"].sum().sort_values(ascending=False)


df.sort_values(by="Revenue", ascending=False).head(10)


https://colab.research.google.com/drive/1FI4XKUkF8G3_2c6slMgAyr3-qjJwxpMM    - link of google collab
