Comparison of customer sentiments for brewers by Word Cloud
The project consists of comparison of sentiments by customers on the crowd sourced local networking business site, Yelp for two brewers. The Yelp site below is 
![image](https://user-images.githubusercontent.com/40518603/115687412-c5ce4f00-a377-11eb-856a-4956a759b340.png)

 
Data
The data entered is the name of the restaurant and the location in which we search the business. In the example we search for a Yard Brewing Company in location Philadelphia USA.
![image](https://user-images.githubusercontent.com/40518603/115687523-e39bb400-a377-11eb-98f8-6657050d1f2b.png)
 

A customer review is as below 
![image](https://user-images.githubusercontent.com/40518603/115687587-f44c2a00-a377-11eb-89a6-410a70073a56.png)


Workflow
The data entered in the www.yelp.com site.
We check whether the url is responding or not by 
url_1 = 'https://www.yelp.com/biz/yards-brewing-company-philadelphia-3'
response_1 = requests.get(url_1)
if response_1.status_code == 200:
    print("Success")
else:
    print("Failure")

We parse the data by using package BeautifulSoup  and using html.parser
To display the response in a form of word Art we use word cloud to emphasize the most frequent word. The more frequent the word is used the bigger is the size of the word.
Below is the comparison of two brewers 
1)	Yard Brewing Co
2)	Philadelphia Brewing Co
 
![image](https://user-images.githubusercontent.com/40518603/115687619-ff9f5580-a377-11eb-96aa-b5a431b9b640.png)
