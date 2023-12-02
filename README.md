# Python-Web-scraping-
Company domain by Company Name 
import pandas as pd

filename = "/content/sameep.csv"
df = pd.read_csv(filename)
df2=df.iloc[:,0]
try:
    from googlesearch import search
except ImportError:
    print("No module named 'google' found")

# to search
for i in df2:
  for j in search(i, tld="co.in", num=1, stop=1, pause=2):
    print(j)
