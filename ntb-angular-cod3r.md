# Angular 9 - Essencial COD3R

https://github.com/isaiaszanoni/Angular-9-essencial.git





# Backend

Vamos utilizar o JSON Server para simular um ambiente backend. Ele lê um Json e cria uma API baseada nele. Neste objeto constará todos os endpoints da nossa API.

`npm i -y` - Vai criar um arquivo package.json, onde podemos incluir as nossas dependências. O `-y` serve para responder todas as perguntas como yes.
`npm i json-server` - Vai instalar a dependência e já colocá-la dentro do arquivo package.json.

Vamos criar um arquivo chamado `db.json`

```json
{
    "products": [
        {
            "id": 1,
            "name": "Caneca BIC preta",
            "price": 2.25
        },
        {
            "id": 2,
            "name": "Caneca BIC azul",
            "price": 2.25
        },
        {
            "id": 3,
            "name": "Caneca BIC vermelha",
            "price": 2.10
        },         
        {
            "id": 4,
            "name": "Caderno Escolar Frida Khalo",
            "price": 21.50
        }
    ]
}
```



\- Agora vamos criar mais um script dentro do no arquivo `package.json`:

```json
(...)
"scripts": {
 	"start": "json-server --watch db.json --port 3001"
 }
```

