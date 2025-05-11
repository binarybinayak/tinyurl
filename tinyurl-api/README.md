# TinyURL api

## authRouter

- POST /signup
- POST /login
- POST /logout

## urlCompressRouter

# TinyURL API

## authRouter

- POST /signup
- POST /login
- POST /logout

## urlCompressRouter

- POST /compress  
   **Request:**  
   `{ 
  password: { enabled: true/false, password },  
  expiry: { maxCLicks, expiresAt },  
  metaData: { title, description, image },  
  validFrom,
  block: { ip, location },  
  customAlias (need logged in user) 
}`  
   **Response:**  
   `{ shortURL, qr, meta: { title, description, image } }`

## redirectRouter

- GET /redirect/:shortURL
- GET /preview/:shortURL
