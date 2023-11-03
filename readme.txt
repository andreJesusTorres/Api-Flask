[GET: Traer una persona]

curl --location --request GET 'http://localhost:5000/personas' \
--header 'Content-Type: application/json' \
--data '
'

[POST: Buscar una persona]

curl --location 'http://localhost:5000/personas/buscar' \
--header 'Content-Type: application/json' \
--data '{
"dni": "18223847"
}
'

[PUT: Editar una persona]

curl --location --request PUT 'http://localhost:5000/personas' \
--header 'Content-Type: application/json' \
--data-raw '{
"dni": "44247798",
"nombre": "André",
"apellido": "Torres",
"email": "andre.torres@outlook.com.ar"
}
'

[POST: Buscar una persona por su dni]

curl --location 'http://localhost:5000/personas/buscar' \
--header 'Content-Type: application/json' \
--data '{
"dni": "18223847"
}

[DEL: Eliminar persona por su dni]

curl --location --request DELETE 'http://localhost:5000/personas/borrar' \
--header 'Content-Type: application/json' \
--data '{
"dni": "18223847"
}
'

[Base de datos: persona/persona/id-nombre-apellido-dni-email]