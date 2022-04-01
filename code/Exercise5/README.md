# Code for the TCC javaparser

This project's purpose is to iterate througth another project repository and compute the Tight Class Cohesion of each class.

It creates a csv file containing 3 colums : "class","package","TCC". I have used this file to create histograms using python. 
```
df = pd.read_csv("TCCReport.csv")
df=df.sort_values("TCC")
sb.barplot(data=df, x="class",y="TCC",color="Black")
```

The two histograms that I have created correspond to the TCC values of the *common-collection* repository and the *common-lang* repository.

![This is an image](https://github.com/MatilinThomas/VV-ESIR-TP2/edit/main/code/Exercise5/commonCollectionHistogram.png)

