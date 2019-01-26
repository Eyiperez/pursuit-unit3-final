# Pokemon API
[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/bfd492a0ffb5b74d963e)
## Models:
- Trainer
  - id
  - name
  - hometown_id
- Town
  - id
  - name
- Pokemon
  - id
  - trainer_id
  - name
  - type_1
  - type_2
  - level


### Town:
- `GET /town/:name/trainers/`: Gets all the trainers from that hometown

### Trainer:
- `POST /trainer/`: Creates a new trainer
- `GET /trainer/:name`: Gets the trainer with the name
- `PUT /trainer/:name`: Updates the trainer with the name
- `DELETE /trainer/:name`: Deletes the trainer with the name
- `GET /trainer/:name/pokemons`: Returns all the pokemon owned by trainer
- `GET /trainer/:name/pokemons?levelmin=50`: Returns all the pokemon owned by trainer greater or equal to level

### Pokemon:
- `POST /pokemon/`: Creates a new pokemon
- `GET /pokemon/:id`: Gets the pokemon with the id
- `PUT /pokemon/:id`: Updates the pokemon with the id
- `DELETE /pokemon/:id`: Deletes the pokemon with the id
- `GET /pokemon/:type/all`: Returns all pokemon of that type from either type_1 or type_2 
