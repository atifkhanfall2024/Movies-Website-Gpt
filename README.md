
# NETFLIX GPT

 - first we create an react app 
 - tailwind installation
 - Header
 - Login
 - signin/signup
 - Routing 
 - Form handling
 - use Ref hook
 - Firebase authentication
 - Sign in and sign up with full authentication
 - Firebase authentication
 - Redux sotre
 - add slices adduser slice remove user slice 
 - then use instead of dispatch we are use an api of firebase onauthstatechange and then use diaspatch to dispatch its value into store
 - use of provider in main app
 - successful login goto browse page
 - Also add signout function
 - useNavigation hook
 - OnAuthChange => this api is actually called when we sign in  ,out , or up outomatically called this api
 - bug fix of user onAuthstatechange
 - redirect user if user is not login donot go to browser page using localhost:3000/browse on this redirect back to login when the user is not login 
 - unsubscribe => i use unsubscribed when i want to unmount the onauthchange call back
 
 
 # Browse Page 
 - Main container
   - Movie background
   - movie title
 - secondary container
  - movies * n rows
    - cards  *n in each row

# Main COntainer Flow
 * in main container i have call an api of now playing movie and get all the information from all the movie then send props for these  in title and background 
   
   # title 
    - in title i have pass props of movie title and description 

    # background 
    - in background file i have make an api call of moives and then filter it if filter moive is find in first index then give me other wise give me next movie background 
    - usage of iframe inside background 
    

  # Main container
 - Title
  - inside it i pass props inside it take title and review of movie
 - background
  - in background i fetch an api from movie data base then after this i use filter method that if vedio is present of trailer then give me other wise give me the json.result specific vedio
  - then i use trailer and set a state inside it and that triler key push into iframe src to display this vedio 
 - movie slice
  - create a movie slice initally null then calling an api of movies now plying name and dispatch it into store 
  - then we read that movie in title.js from this we read title and review 
  
  - creating custom hook for code reusability and cleaning code


# Features 
 signin / signup forms
 after login browser page

# browser page
  Header
  Main movie
  background trailer
  description and title
  Buttons
  Movie suggestion
  Movie list *N  


  # Working on Secondary container

   - secondary container
     - movie list
     - movie cards

 -  In secondary container i  have made a call of the movies that have already in store 
 - Then passing props of that movie inside in movielist and movie cards 
 - I set multiple call of list in Secondary container 
 - movie list read title and movies passing as a props inside it so we need an img of movie inside cards so we extract its image from movies and send in movie card file 
 - we also set map on movie card because we have multiple movies 

 # usage of cloudinary of tmdb inside project
 - inside in movie cards i have make an  api call of cloudinary link and and image path that we extract it add with them
 - Usage of scrollbar concept 



 # ALso add some other movies Slices
 - call some apis and push that api movies data into store and use in secondary container 


 # Add link
 - add some links on header 


 # Header updation

 - today i duild a feature that when a use onauth success then i use a state varaible that setuser is not user so now its is not show image signout and gpt in ligin page its only show in browse page
 - use state variable const [isuser , setisuser] = usestate(false)


 # GPT Working 

 - so we have start working on gpt inside gpt have two components search gpt and movie suggestion
 - i export gpt in browse
 - now i work on hanlde the toggling on gpt button that when i clicked on button then toggle the page to gpt page
 - so i create a slice for toggling that when i clicked on button then dispatch its value to store and read this value in browse page that when showme is true then show me page other wise donot show me gpt page

 - after that i build seach bar gpt 

 # Multilanguage 
 - create multi_ Language  fully working
 - some languages i used to change when the user want to change something maen languages 

# GPT API 

- so i use openai api use today working of it really amazing that when i search movies it give me those movie which i want for example if i want to search funniest movies so it give the recommended movie 

- using of tmdb search movie api its working really amazing 

also on backgrouund dynamic vedio change work on ai based