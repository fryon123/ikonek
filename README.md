# Welcome to I-Konek!
I-konek is derived from bisayan pronouncation of connect. Ikonek means "to connect".
I-konek aims to bring the convenience of remote job finding to every corner of the country, with high of low connection signal. 

## How it works
I-konek will be designed based on the modern online job finding platforms. The only difference of I-konek from the other services is it's accessible by everyone! Philippines is an island, therefore, it is composed of huge and beautiful landmasses. This landmasses, even though it is refreshing to our eyes, is a burden in providing fast internet to the people that are living in these places.

I-konek will solve this problem by utilizing the SMS (Short Messaging System) as a medium between the job finders and the service. SMS can be used without internet and with little signal. With this approach, wider group of people can experience the convenience of remote job finding.

**I-konek** is composed of three(3) components: 
- **Website**
- **SMS Gateway**
- **Backend Server**

##Website
The website will serve as the between the employer and the employee. The employers can search for a job they want to hire and the website provides them employees that can be contacted  immediately with a click of a button. This is the front-end.
##SMS Gateway
This component will handle every communication that includes the use of SMS. This will serve as a gateway between the job finders and the service. Because of expensive SMS Services, I-konek uses an app developed using [Flutter](https://flutter.dev "Flutter") that will handle text messages.
### Backend Server
This is the main component of I-konek. This serves as the "provider" of I-konek. The backend server will provide the necessary data that are being requested by other components.  This component is also the one that communicates to the database. I-konek uses [Firebase](http://firebase.com "Firebase") for storing every data. The backend server uses glitch for the meantime as a hosting service. In the future, the server should be migrated to [Google Cloud](https://cloud.google.com/nodejs/ "Google Cloud").

> I-konek also uses Firebase Cloud Messaging (FCM) for direct communication between the Backend and the SMS Gateway.

I-konek is utilizing the use of **[REST](https://www.ibm.com/cloud/learn/rest-apis "REST")** API for communication between the server and its components.
#### Try it in your browser
You can use the website protoype. https://clean-fishy-honeydew.glitch.me

**REST Endpoints**
In your browser, enter the following to test it.

`https://clean-fishy-honeydew.glitch.me/jobs/programming`
It will return the job finders' names with that skill, in this case, programming.
You can search for other jobs. Try *mowing*.

`https://clean-fishy-honeydew.glitch.me/profile/ FRYON AMBOY` <- include the spaces
This will return a specific profile.

> Due to limited resources, we can't make the I-konek's SMS Gateway turned on always. 

#### Try I-Konek on your SMS Capable phone
Send any text message on this Mobile Number: **+639687227109*
Our automated text responder will help you out in using our service.

## Sources
[fryon123/ikonek-server](http://github.com/fryon123/ikonek-server "fryon123/ikonek-server")
