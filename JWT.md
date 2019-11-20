### JWT Detalle

* Para armar el token: https://jwt.io/ 
* Datos
  * SECRET: Klave muy secreT4
  * sub: subject (usuario del sistema) user1, user2, admin
  * admin: indica si es administrador del sistema (agregado en el response)
* Ejemplos
 
 * Token: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJ1c2VyMSIsIm5hbWUiOiJVc3VhcmlvIDEifQ.p-81M-mAceOS-m3RR8_TfVDd6p5YqPJtIcyZz3SlxLg
  * Contenido: { "sub": "user1", "name": "Usuario 1" } Este MS agrega "admin": false
 
 * Token eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJ1c2VyMiIsIm5hbWUiOiJVc3VhcmlvIDIifQ.EiKdTPpiqkrb-Tae--0qMflu0IYlqGGkOxWK1RBRNMo
  * Contenido: {"sub": "user2","name": "Usuario 2"} Este MS agrega "admin": false
 
 * Token: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJhZG1pbiIsIm5hbWUiOiJhZG1pbmlzdHJhZG9yIn0.QNQ1rqU8a4tu5bCPGmgKZi1lIQz5V61ia0BfOsZz438
  * Contenido: {"sub": "admin","name": "administrador"} Este MS agrega "admin": true
