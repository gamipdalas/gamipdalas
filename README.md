version: "2.0"
intents:
  - greet
  - goodbye
  - inform
  - request_info

entities:
  - name
  - location

slots:
  name:
    type: text
  location:
    type: text

responses:
  utter_greet:
    - text: "¡Hola! ¿Cómo puedo ayudarte hoy?"
  utter_goodbye:
    - text: "¡Adiós! Que tengas un buen día."
  utter_ask_name:
    - text: "¿Cuál es tu nombre?"
  utter_ask_location:
    - text: "¿Dónde te encuentras?"

actions:
  - action_provide_info
