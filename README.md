# spotify-web-api-react-rails-auth-code-flow-demo

A simple template for pure React JS 
VERY bare boned functional React front end/ Ruby on Rails backend using the Spotify Web API's Authorization Code flow.
Got some JWT tokens in there as well
Just fetches user info, but is all you need to get started without enduring the frustration and embarassingly long, endless hours I suffered through...
Just clone and get started! The Authorization Code flow is seriously the most difficult part of working with the API in order to access user data and utilize web tokens.

To mess around, you need a Spotify account in order to get some credentials for the "AUTHORIZATION CODE FLOW" (1st of 3 auth options)

I used FIGARO gem to hide these codes so you can fill in the 
1) client_id: '<your client_id>'
2) client_secret: '<your client_secret>'
3) redirect_uri: 'http...' <--- this is the callback uri you need to get to the auth page

and JWT: (add <gem 'jwt'> to gemfile)

1) a secret key
2) an algorithm

if you do use Figaro, add <gem 'figaro'> to gemfile
- and after bundle installing the gemfile, make sure to enter < bundle exec figaro install > in the terminal so you can store your secret info in the newly created config/application.yml file

add < gem 'rest-client' > to assist in making requests to/from API
