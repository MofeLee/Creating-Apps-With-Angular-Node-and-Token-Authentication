# Creating-Apps-With-Angular-Node-and-Token-Authentication
[Pluralsight] Creating Apps With Angular, Node, and Token Authentication [2014, ENG]




### 02. Register in Front End Views  

02. Register in Front End Views | 05-Environment Setup  

yum install -y libpng-devel  


npm install -g nodemon  
npm install -g yo  
npm install -g bower  
npm install -g grunt-cli  
npm install -g generator-angular

yo angular  

? Would you like to use Sass (with Compass)? (Y/n) n  
? Would you like to include Bootstrap? Yes  
? Which modules would you like to include?  Nothing


grunt serve

http://localhost



02. Register in Front End Views | 06-Generated Angular Project  

Nothing  

02. Register in Front End Views |  07-Register View

yo angular:view register  


02. Register in Front End Views |  08-ui-router

bower install --save angular-ui-router

http://localhost/#/  
http://localhost/#/register


02. Register in Front End Views |  09-App Theme

http://bootswatch.com/

Theme: SuperHero


http://bootsnipp.com/snippets/featured/login-screen-with-background



02. Register in Front End Views |  10-ui-sref active


02. Register in Front End Views |  11-Register View Fixes



### 03. Register Front End Controllers and Services

03. Register Front End Controllers and Services | 14-Match Password Directive  

yo angular:directive validateEquals  


03. Register Front End Controllers and Services | 15-Register Controller  

yo angular:controller register  

По нажатию на Submit, в консоль пишется "test"  


03. Register Front End Controllers and Services | 16-HTTP Post

Nothing


03. Register Front End Controllers and Services | 16-HTTP Post

bower install --save animate.css
yo angular:service alert


03. Register Front End Controllers and Services | 17-Alert Service

Неудачная попытка регистрации в системе.



### 04. Register WebAPI Manual JWT

04. Register WebAPI Manual JWT | 20-API Environment Setup  

mkdir frontend  
mkdir api  

Все кроме git в /frontend  
cd api/  

npm init  
npm install --save express

nodemon api.js

С помощью PostMan делаю POST запрос localhost/register
получаю ответ.


04. Register WebAPI Manual JWT | 21-API Register Post  

cd api/  
npm install --save body-parser  

nodemon api.js


04. Register WebAPI Manual JWT | 22-MongoDB Save User


cd api/  
npm install --save mongoose  

nodemon api.js


04. Register WebAPI Manual JWT | 23-Encrypt Password With Hash

cd api/  
npm install --save bcrypt-nodejs  


04. Register WebAPI Manual JWT | 24-Hide Password  


04. Register WebAPI Manual JWT | 25-JWT Encoding From Scratch  

cd api/  
npm install --save crypto  

nodemon api.js
eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.ImgxIg==.WkzcmKyO2ZLVkHGnH2fzuv2eVuRqadfCYqfuEMC5IJo=


04. Register WebAPI Manual JWT | 26-Token Passed With Register  


04. Register WebAPI Manual JWT | 27-Authtoken Factory  

cd frontend/
yo angular:factory authToken

04. Register WebAPI Manual JWT | 28-isauthenticated

cd frontend/  
yo angular:controller header



### 05. Register WebAPI JWT Library

05. Register WebAPI JWT Library | 31-Logout

cd frontend/  
yo angular:controller logout  


05. Register WebAPI JWT Library | 32-Jobs and Greetings


cd frontend/  
yo angular:controller jobs


05. Register WebAPI JWT Library | 33-View Animations  

cd frontend/
bower install --save angular-animate


05. Register WebAPI JWT Library | 34-Securing the Jobs Resource

Nothing

05. Register WebAPI JWT Library | 35-Auth Interceptor

yo angular:factory authInterceptor


05. Register WebAPI JWT Library | 36-JWT Decoding From Scratch

Nothing

05. Register WebAPI JWT Library | 37-Verifying the Signature

Nothing

05. Register WebAPI JWT Library | 38-Design Break Optimize Alerts

Nothing


05. Register WebAPI JWT Library | 39-Switching to Node JWT Simple

cd api/
npm install --save jwt-simple  



### 06. Login


06. Login | 42-Login Endpoint

Nothing  

06. Login | 43-Login View


cd frontend/  
yo angular:controller login  
