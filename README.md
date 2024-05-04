# gptProjectv1

I will guide you to run the  dockerized version of this project on your device 
<img width="621" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/9a6a10d7-90e9-47c8-924c-5900d2590132">

I deployed the image of the dockerized version of this project in the docker hub repository that I created with my docker account
<img width="1299" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/0af76271-2d62-4856-b1ae-5cbe4a96f95c">

I will guide you to run the image on your device 

first you need to install docker desktop 
then you need to run on the terminal this command:    docker pull amineleny3/gpt:v1

right now you have the image downloaded on your device 

to run the container you need to run this commande : docker run -d -p 8000:8000 --name containername  amineleny3/gpt:v1 

now you need to go and look for containers in the side bar of your docker desktop app 

in this example i remplaced the "containername" in the command"docker run -d -p 8000:8000 --name containername  amineleny3/gpt:v1 "  by "chatgptmicroservice" 
<img width="1434" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/e9a7b841-eb71-48cd-a7a0-1a46f5670dd6">

then click on 8000:8000 port so you can open the localhost page

<img width="1315" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/33f8f658-1428-466f-9ed7-9ddc37cbf10f">

now add /docs to your Url to access the swagger UI so we can do some test (post requests)




<img width="1317" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/cdf2bcb9-d769-4212-9d5b-ec73a9d82121">


now click on the green post

<img width="1328" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/33100d4f-bfb3-4dc7-b1d7-10a78ff7a135">

click on TRY IT OUT 

<img width="1307" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/cc72e8b3-c7b5-409e-8683-4e8d2fb7da99">


and then input the question that you want chatgpt to answer and click on execute


<img width="1312" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/fc1eaa1b-8725-4076-902f-606725fb9f76">


as you can see here we got the wanted data from chatgpt successfly

<img width="1272" alt="image" src="https://github.com/AmineLeny/gptProjectv1/assets/72925780/4dfdebf4-ac57-4491-9210-6cb481ec758e">



















