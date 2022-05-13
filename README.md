# online-shop
Online shop using Django


### How to run the app ?
-------------------------------------

- create a ```venv```  
```$ python -m venv venv```  
activate the venv ```$ venv\Scripts\activate```  
- install all dependencies in ```requirements.txt```  
```($ venv) pip install -r requirements```
- create a ```.env``` file contains Django SECRET_KEY & DEBUG
- to run the server
```($ venv) python manage.py runserver```  
then [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

--------

- Homepage  


  ![homepage](https://user-images.githubusercontent.com/73492002/168231019-22af3118-f4e2-4ed1-820f-c3d5cc400964.png)


- Cart  
  copouns system is working via adding code and getting discount for total price in cart


  ![cart](https://user-images.githubusercontent.com/73492002/168231203-6acbbdd4-7065-4cbd-8278-47fc6fa8c2fe.png)


- place order  
  after placing order email is sent asynchronously via celery  
  
  
  ![place order](https://user-images.githubusercontent.com/73492002/168232015-b5939b0c-1796-4ae6-bc16-0f902b037a7f.png)
  
  
 - check out
   payments is managed by braintree  
   make to sure to add BRAINTREE_MERCHANT_ID, BRAINTREE_PUBLIC_KEY, BRAINTREE_PRIVATE_KEY in the ```.env``` file
   
    
   ![pay](https://user-images.githubusercontent.com/73492002/168236599-613d231a-19a1-47b2-a6c3-da2dd4a135ad.png)

   
