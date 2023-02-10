# ChromeExtension
The purpose of this chrome extension is to provide user the interface to put their details and invitation code required to start the online exam conducted by elitmus.
Basically , this extension is provided with some functionality such that it will start interacting with user directly by just clicking on it(extension). Then user will be prompted to allow the permissions of audio and video i.e. after the submission of the user details form.

******
Not up to the Mark:
Since, the functionality of taking the user permission for audio and video access is not implemented So, I am not able to proceed further, i.e. taking the screenshot part. 
Problem: I have created the the form for user details in "userForm.html" file where there is a button which I have to click and it will redirect to the "media.html" page. But, unfortunately the page is not redirected i.e., after clicking "Start Test" button nothing actually happens. Both "media.html" and "media.js" file will work fine when I try to run it separately apart from the extension.
***
Intuition behind solving the above problem(not yet solved): I have just make other web page i.e. userForm.html in browser by just using chrome_overrides Since the DOM of the web page is manipulated using content_script. But when I try to redirect the current DOM to "userForm.html" it via making "content.js" page in content_script then also it is doing nothing. 
Since I have used the interaction between "popup.html" and the "userForm.html" by just using another file "redirect.html" which basically redirect to the new tab containing the data of "userForm.html" using meta tag refresh property. And since the "userForm.html" file is a part of DOM so my intuition says that this should again redirect to "media.html" using convetional javascript method of redirecting. But it doesnt work.
***
Since the frontend part is not completed so I not go for the development of backend i.e., fetching the data into the database. But I have done this type of activity previously which You can see in my git repository.
