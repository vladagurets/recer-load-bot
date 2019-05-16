# Bot for user activities simulator.

Uses for load-tesitng of sharedb server.

- npm install / yarn
- starts with prefered params
  - *wsUrl* (url of ws connection)
  - *collections* (prefered collections for CRUD actions)
  - *connections* (amount of generated instanses)
  - *lifeTime* (time of user's session in minutes)

*Example:*  ```node index wsUrl=wss://my-example-app.io/ws connections=100 collections=images,files,users lifeTime=5``` 
- It'll generate 100 *user's* connection
- Each user will interact with random collection from *collections* param for user's *lifeTime* session



TODO:
  - Add create, update, remove actions
  - Add logs for average actions count per minute