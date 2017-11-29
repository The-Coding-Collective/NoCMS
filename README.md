# NoCMS
This system can create a website based on all the (social) information already shared on the internet.

Each time I'm working for a client I will get these questions where they want newsitems on the website, with an image, title, description.
On publishing the newsitem in the CMS, they'll want the newsitems to be published to twitter and facebook as well.

Why not use it the other way around? You're essentialy making the social channels a CMS this way.
And content managers are already very familiar with these systems. This way Content managers don't have to be trained on a new system.
Another plus is that there's already lots of information available on these channels.

Based on .NET

Consist of two seperate systems, the frontend and backend.


**BACKEND**
The backend will be the system where pages can be created, components can be dragged and dropped on each page.
Per component a different datasource can be configured.

a datasource will include a OAUTH provider and the appropiate method to retrieve data.

OAUTH providers can be configured with the correct keys.

The data from the backend will be provided through a webapi in the form of JSON.

**FRONTEND**
The frontend will be the website itself. Based on MVC.

On rendering the website will retrieve the JSON for the page through a WEBAPI call.
Then it will do the OAUTH calls to the OAUTH providers of each component.
On receiving the data, the components will be rendered.
