# Chat API

### Url base: http://localhost:9000/api/v1

- /auth
    - /login -> Login con las credenciales del usuario para autenticar

- /conversations
    -post  -> Crear una nueva conversacion 
         
    -get
        /:conversation_id  -> Mostrar conversaciones del usuario loggeado.
        /:conversaton_id/messages  -> Mostrar los mensajes de una conversacion
        /:conversation_id/messages/:message_id  -> Obtener mensaje de una conversacion por id.
    -patch
        /:conversation_id  -> Si eres administrador puedes editar esta conversacion.  
    
    -delete
        /:conversation_id  -> Eliminar mis mensajes
        /:conversation_id/messages/:message_id  -> Eliminar mensaje de una conversacion por su id.

- /users
    -get 
        /me  -> Obtener mis usuarios.
        /:id  -> Obtner usuario por su id.
    -patch
        /me  -> Editar mi usuario.
        /:id  -> Editar cualquier usuario por su id.
    -delete
        /me  -> Eliminar mi usuario.
        /:id  -> Elimina usuario por su id.
  

