# Proyecto_datalake
# PULSO POLITICO
# TWITTER > COUCHDB > MONGODB > POWERBI

![image](https://user-images.githubusercontent.com/74762981/156109950-6d96ef51-809a-49cf-bc25-b0786f572fa1.png)

- Para realizar la extraccion de datos instalaremos los paquetes de twitter e importaremos las 
siguientes librerias

![image](https://user-images.githubusercontent.com/74762981/156109915-16f905c8-bbe2-417a-8a29-06525c5e6457.png)

- Para realizar el analisis de datos en twitter es necesario trabajar con las api keys proporcionadas por la platafoma
,una vez implementado crearemos una clase LISTENIR y un objeto STREAM la cual son funciones utilizadas con la libreria tweepy para el analisis de los datos

![image](https://user-images.githubusercontent.com/74762981/156111207-200d8f9c-373b-49fc-8d92-25180c712365.png)

- Crear una transmision para utilizar las api keys

![image](https://user-images.githubusercontent.com/74762981/156111521-fe619de9-629d-49b4-8e5f-913ca8405b4a.png)

- Realizar la conexion con la 1era base de datos Couch Db.
- Ingresando usuario,clave y el puerto con el que realizara la conexion
- Se debe ingresar la base de datos a crear 

![image](https://user-images.githubusercontent.com/74762981/156112229-7e37fd8a-1662-4595-8bd4-4143643b502e.png)
![image](https://user-images.githubusercontent.com/74762981/156113194-9ca13457-e41e-4f77-80e8-ede53615e836.png)

- Mediante tweets buscados en la red podemos visualizar informacion mediante el id de presidentes o noticias 
de varios paises ,para ingresar en el filtro a buscar.

![image](https://user-images.githubusercontent.com/74762981/156112837-7f238635-28a1-4f70-824c-3a5cdaacd673.png)
- Ingresamos en el filtro todos los campos comentados anteriormente ,para tranasladar la informacion ala base de datos de COUCH DB
![image](https://user-images.githubusercontent.com/74762981/156112963-ba3c8fce-72f5-45b2-9261-b49a96ccdecf.png)

- Una vez terminado de buscar los tweets e importado a couch db procedemos a tranasladar al concentrador MONGODB
- Importamos las librerias de Mongo DB

![image](https://user-images.githubusercontent.com/74762981/156113508-b0099e85-e415-4913-870c-a371ebd4e685.png)

- Realizamos las conexiones con la base de datos que va a transmitir la informacion a MongoDB
![image](https://user-images.githubusercontent.com/74762981/156113632-3edb4f66-86c0-48bf-adc5-736ce028adc3.png)

- Establecer los parametros que recibira la base de datos

![image](https://user-images.githubusercontent.com/74762981/156113714-cd56afbf-2215-4a93-9fec-8c6e2f436de4.png)

- Ingresamos la base de datos de CouchDB

![image](https://user-images.githubusercontent.com/74762981/156114163-9604443a-3ddc-4bf6-a0a8-23725a1884a8.png)

- Ingresar el servidor de mongoDb mediante una funcion llamada mongoclient.
- Ingresamos el Ip y el puerto
- Verificamos que la conexion sea exitosa y crear la base de adtos y la coleccion

![image](https://user-images.githubusercontent.com/74762981/156114392-06d62ee9-258f-492d-a3d4-970c7f4b467a.png)

- Implementar un ciclo for que permite el traspaso de datos a mongoDB

![image](https://user-images.githubusercontent.com/74762981/156114474-ee8aac69-2d33-48ab-8a93-1d21d8fe9442.png)

-Conexion exitosa con las dos base de datos

![image](https://user-images.githubusercontent.com/74762981/156114535-c6df1dbb-e2b7-4d4d-9fd6-ccac7c010f48.png)

-verifiamos la base de datos y su coleccion creada dentro de MongoDb

![image](https://user-images.githubusercontent.com/74762981/156114795-f27beed9-aca4-42a9-a3cb-f3f1f227069c.png)

![image](https://user-images.githubusercontent.com/74762981/156114860-91648878-c817-4f54-b9e0-3ec249f2b0c6.png)


- Una vez diseñada la arquitectura, verificaremos que en MongoDB se encuentren nuestros datos.

- Para el siguiente paso es extraer estos nuevos datos como csv y los enviaremos 

![image](https://user-images.githubusercontent.com/74762981/156110534-39b8df4a-dd30-4050-968b-5b1d26a8d616.png)
![image](https://user-images.githubusercontent.com/74762981/156110617-c74e3799-a95b-4de3-9581-8a18af453ccc.png)

- Como ultimo paso cargaremos el nuevo csv dentro de POWERBI

![image](https://user-images.githubusercontent.com/74762981/156116104-ce28dce1-2d14-441a-910e-af5efe5acbf6.png)

- Seleccionamos la tabla importada
- Seleccionamos un indicador para visualizar los datos

![image](https://user-images.githubusercontent.com/74762981/156116285-a3e064c8-1d98-4bdd-93f5-2db77a6b8c7c.png)

- Mostramos Indicador - MAPA

![image](https://user-images.githubusercontent.com/74762981/156116350-a94fe8da-865f-422f-a551-2cfcb86db602.png)

- Podemos verificar el uso de la aplicacion el analisis de datos mediante varios paises y su fiabilidad al momento de realizar extraccion de datos mediante un perfil o cadenas de texto.

# COVID
# FACEBOOK > COUCHDB > MONGODB > POWERBI

![image](https://user-images.githubusercontent.com/74762981/156117215-bb32cc5f-4b4f-43e9-bd5c-157c4768fb09.png)

- Para realizar busquedas y analisis de datos es necesario instalar los paquetes de facebook scrapper


![image](https://user-images.githubusercontent.com/74762981/156117549-b1334f35-0d60-43a6-861d-f0359e40c342.png)

- Importar librerias de facebook y de la base de datos a utilizar 

![image](https://user-images.githubusercontent.com/74762981/156117832-a8fee2f6-5ef7-493f-9626-b1908f0edb99.png)

- Realizamos la conexion y creamos la base de datos

![image](https://user-images.githubusercontent.com/74762981/156118284-22fef075-7712-4a95-bfba-a50e13433514.png)

- Realizamos la busqueda en paginas especificas sobre covid de varios paises y cada una empezamos a verificar si hay publicaciones del tema.

![image](https://user-images.githubusercontent.com/74762981/156118399-8f6604fc-14ce-449c-9781-7a343338de3e.png)

- Creamos un ciclo de repeticion donde ingresara la pagina como parametro.
- Ingresaremos el numero de paginas que se deseen extraer la informacion

![image](https://user-images.githubusercontent.com/74762981/156118856-17baced2-90cc-413e-9e18-11893efde5ed.png)

- Creamos un Diccionario la cual va almacenar cada reaccion, likes,etc que obtendra de las publicaciones de facebook.

![image](https://user-images.githubusercontent.com/74762981/156118955-4679c9b4-a876-4f54-9a83-8c1e01945cb4.png)

- Implementamos una linea de codigo donde realizaremos el tratamiento de errores de facebook
- Utilizando el diccionario creado se ira guardando la informacion que va extrayendo facebook de sus publicaciones

![image](https://user-images.githubusercontent.com/74762981/156119234-844fcb71-1f88-4c65-92dc-1024cd87bef5.png)

______________________________________________

- Importamos las librerias de Mongo DB

![image](https://user-images.githubusercontent.com/74762981/156113508-b0099e85-e415-4913-870c-a371ebd4e685.png)

- Realizamos las conexiones con la base de datos que va a transmitir la informacion a MongoDB
![image](https://user-images.githubusercontent.com/74762981/156113632-3edb4f66-86c0-48bf-adc5-736ce028adc3.png)

- Establecer los parametros que recibira la base de datos

![image](https://user-images.githubusercontent.com/74762981/156113714-cd56afbf-2215-4a93-9fec-8c6e2f436de4.png)

- Ingresamos la base de datos de CouchDB

![image](https://user-images.githubusercontent.com/74762981/156119728-aa22859e-dd1d-420a-bcc8-c8142291d835.png)

- Ingresar el servidor de mongoDb mediante una funcion llamada mongoclient.
- Ingresamos el Ip y el puerto
- Verificamos que la conexion sea exitosa y crear la base de adtos y la coleccion

![image](https://user-images.githubusercontent.com/74762981/156119802-50cbd860-6107-4696-851c-5cc74b4700bd.png)


- Implementar un ciclo for que permite el traspaso de datos a mongoDB

![image](https://user-images.githubusercontent.com/74762981/156114474-ee8aac69-2d33-48ab-8a93-1d21d8fe9442.png)

-Conexion exitosa con las dos base de datos

![image](https://user-images.githubusercontent.com/74762981/156114535-c6df1dbb-e2b7-4d4d-9fd6-ccac7c010f48.png)

-verificamos la base de datos y su coleccion creada dentro de MongoDb
- Una vez diseñada la arquitectura, verificaremos que en MongoDB se encuentren nuestros datos.

![image](https://user-images.githubusercontent.com/74762981/156119917-4237b155-e500-4f86-ac87-38024f16348c.png)

![image](https://user-images.githubusercontent.com/74762981/156119975-01a8bd50-4d4a-463b-bc46-e2272c6cb150.png)

- Para el siguiente paso es extraer estos nuevos datos como csv y los enviaremos 

![image](https://user-images.githubusercontent.com/74762981/156110534-39b8df4a-dd30-4050-968b-5b1d26a8d616.png)
![image](https://user-images.githubusercontent.com/74762981/156110617-c74e3799-a95b-4de3-9581-8a18af453ccc.png)

- Como ultimo paso cargaremos el nuevo csv dentro de POWERBI

![image](https://user-images.githubusercontent.com/74762981/156116104-ce28dce1-2d14-441a-910e-af5efe5acbf6.png)

- Seleccionamos la tabla para visualizar y un indicador grafico

![image](https://user-images.githubusercontent.com/74762981/156120322-30aaea1a-be28-43d9-8301-d855d690fc21.png)

![image](https://user-images.githubusercontent.com/74762981/156120368-bd9a1661-ba56-4031-97e1-dbbad5ff1cc3.png)

- Datos analizados con facebook , se logro extraer los likes de cada publicacion acerca de coronavirus y visualizar en POWERBI para analizar
donde fueron hechas las publicaciones y sus diferentes reacciones y comentarios.
______________________________________________

# Juegos
# TWITTER > MONGODB > POWER BI

- Importamos librerias de Twitter y mongoDb

![image](https://user-images.githubusercontent.com/74762981/156123992-0376db03-aaac-43a1-b39f-36bc02d27f3a.png)

-Creamos los metodos para autenticar e ingresar las api keys

![image](https://user-images.githubusercontent.com/74762981/156124114-48cec9d0-d53c-44d9-bc88-4e62d3b06d7a.png)
 
- Ingresamos el servidor de mongoDb
- Creamos una base de datos en mongodb
- Creamos una coleccion donde se almacenara los datos

![image](https://user-images.githubusercontent.com/74762981/156124282-d08d01ff-a593-472f-a101-d224a3235f5a.png)

- Ingresamos la cadena de texto a buscar

![image](https://user-images.githubusercontent.com/74762981/156124342-0893c7ef-4e81-4f98-b41b-599fe6444d33.png)

-Mediante la funcion api.search buscara en los tweets la palabra ingresada y lo extraera.

![image](https://user-images.githubusercontent.com/74762981/156124417-53503ba2-a01f-44fe-a943-9ab7c8f74657.png)

-Imprimir los resultados de busqueda

![image](https://user-images.githubusercontent.com/74762981/156124802-c0792cc2-a6a6-4326-be8d-e19e7e543943.png)

- Obtenemos los estados
- Mostramos e imprimimos los estados.

![image](https://user-images.githubusercontent.com/74762981/156125015-f58a2e32-c368-4d46-af4c-ba8d5a336ba4.png)

- Generamos un ciclo para imprimir los metadatos y resultados de busqueda

![image](https://user-images.githubusercontent.com/74762981/156125223-c9768f28-819b-4f3f-874b-2efb709b0832.png)

- Datos recopilados a mongo Db

![image](https://user-images.githubusercontent.com/74762981/156125433-c696af42-f60b-4f10-b08c-0a366cd48343.png)

- verificamos la base de datos y su coleccion creada dentro de MongoDb
- Una vez diseñada la arquitectura, verificaremos que en MongoDB se encuentren nuestros datos.

![image](https://user-images.githubusercontent.com/74762981/156125737-2df9a56b-7987-4474-99d3-67271a94a33c.png)

![image](https://user-images.githubusercontent.com/74762981/156125793-678c312b-80e3-4714-b187-3c441fb3d26b.png)

- Para el siguiente paso es extraer estos nuevos datos como csv y los enviaremos 

![image](https://user-images.githubusercontent.com/74762981/156110534-39b8df4a-dd30-4050-968b-5b1d26a8d616.png)
![image](https://user-images.githubusercontent.com/74762981/156110617-c74e3799-a95b-4de3-9581-8a18af453ccc.png)

- Como ultimo paso cargaremos el nuevo csv dentro de POWERBI

![image](https://user-images.githubusercontent.com/74762981/156116104-ce28dce1-2d14-441a-910e-af5efe5acbf6.png)

- Seleccionamos la tabla para visualizar y un indicador grafico

![image](https://user-images.githubusercontent.com/74762981/156125848-0451cbdd-5f55-4fc2-9c4a-f43b6617d656.png)

- Se analizaron los datos por paises mediante un mapa y un indicador que muesta cuantos retuiteron
y cuando realizaron publicacion del juego ingresado

