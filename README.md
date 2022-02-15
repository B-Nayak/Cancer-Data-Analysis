# Cancer-Data-Analysis



## Click on the charts below to interact




```python
max_cases=df.sort_values("Total.Number",ascending=False).iloc[0:10,:]
fig = px.bar(max_cases,x='Total.Number',y='State',color_discrete_sequence=['#F83839']*len(max_cases))
fig.update_layout(autosize=False,width=600,height=500)
fig.show()
```
<a href = "https://vigilant-noether-51647d.netlify.app">![](./charts/newplot-10.png)</a>

```python
fig = px.bar(max_rates,x='Total.Rate',y='State',color_discrete_sequence=['#FBEE0F']*len(max_rates))
fig.update_layout(autosize=False,width=600,height=500)
fig.show()
```
<a href = "https://vigorous-colden-a31cb7.netlify.app">![](./charts/newplot-9.png)</a>

```python
fig = px.pie(rate_age,values=rate_age.iloc[0,4:],
             names=['Total < 18','Total 18 - 45','Total 45 - 64','Total > 64'],
             width=600,height=300)
fig.show()
```
<a href = "https://competent-swirles-080b08.netlify.app">![](./charts/newplot-8.png)</a>

```python
fig = go.Figure(data=[go.Pie(labels=male.columns[5:],values=male.iloc[0,5:],pull=[0,0.3,0.1,0])])
fig.update_layout(autosize=False,width=600,height=400)
fig.show()
```
<a href = "https://vibrant-nobel-bf2888.netlify.app">![](./charts/newplot-7.png)</a>

```python
fig = go.Figure(data=[go.Pie(labels=['Breast Cancer','Colorectal','Lung Cancer'],
             values=cancer_type.values,hole=.3)])
fig.update_layout(autosize=False,width=600,height=370)
fig.show()
```
<a href = "https://hopeful-pike-afebb7.netlify.app">![](./charts/newplot-6.png)</a>

```python
fig.layout.margin.update({'t':75, 'l':50})
fig.layout.update({'title': 'Rates of Male vs Rates of Female'})
fig.layout.update({'height':800})
fig.show()
```
<a href = "https://vibrant-joliot-591173.netlify.app">![](./charts/newplot-5.png)</a>

```python
fig = px.bar(min_cases,x='Total.Number',y='State',color_discrete_sequence=['green']*len(min_cases))
fig.update_layout(autosize=False,width=600,height=500)
fig.show()
```
<a href = "https://quizzical-booth-b34ece.netlify.app">![](./charts/newplot-3.png)</a>

```python

<a href = "https://eager-hugle-7a39ff.netlify.app">![](./charts/newplot-2.png)</a>
