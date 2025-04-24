![image](https://github.com/user-attachments/assets/1b5dc6a2-785c-4982-b6ab-9024715f687e)

# Burp Suite Learning Lab

This lab involves accessing online resources to gain practical experience with Burp Suite Community Edition. It includes navigating the interface, learning proper procedures, and understanding which settings to use in various scenarios. There are limitations to the Community Edition (such as the lack of a vulnerability scanner), but I watched videos covering the areas I wasn't able to perform myself.

### Prerequisites
- Computer with Internet Connection
- [Burp Suite Community Edition](https://portswigger.net/burp/communitydownload)
  
---

## Intercept HTTP Requests and Responses
<img width="1000" alt="1" src="https://github.com/user-attachments/assets/9cc331f7-3b59-4e1a-a6ec-03d7b2e86ee1" />

1. Generally begin with HTTP testing, which opens up to other tasks down the road
2. Select Proxy, under the Intercept tab
3. Select Open Browser, Burp Suite will open its embedded browser
4. In this case, we will navigate to [portswigger.net](https://portswigger.net/)

<img width="1000" alt="2" src="https://github.com/user-attachments/assets/d5239fd6-755e-455c-b3de-f8d38558a9a4" />

1. Turning Intercept On, the raw data from the webpage loads into Burp Suite
2. We can read and edit the request, but while intercept is on, the page will be in a constant state of loading

<img width="1512" alt="3" src="https://github.com/user-attachments/assets/2fefa38c-f87b-4800-b92f-897793cb9685" />

1. The options tab allows us to manually configure what gets interecepted
2. We can also apply corresponding rules to the responses

---

## Resend Individual Requests using Burp Repeater
<img width="1000" alt="4" src="https://github.com/user-attachments/assets/0eb6765a-4c39-484c-914f-779a78fd15f8" />
<img width="1000" alt="5" src="https://github.com/user-attachments/assets/6fc1697f-8cf7-4390-9982-d6431e1a7ade" />

1. Easiest way to use Burp Repeater is by sending requests directly to it
2. We can send different requests to the appropriate tools by right clicking on the item we want sent
3. Right click, we see Send to Repeater
4. In the Target tab, select the item of interest, and Send to Repeater

<img width="1000" alt="6" src="https://github.com/user-attachments/assets/694f8c43-e1a5-4703-84e0-8339f89a7d8f" />

1. We can edit the Request side, as well as see the reponse that came back from the server
2. When sending multiple times, we can always return to a previous state using the arrow next to the send button

<img width="1512" alt="7" src="https://github.com/user-attachments/assets/08f5b08b-a123-4c7a-a178-05323d19b1fa" />

1. We can also send redirects, which can be used to see reponses from the server as well
2. Burp allows us to copy-paste a url, which will create its own request, which we can then send to receive a response
