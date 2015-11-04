# Portal de Bitacora


Aplicativo para portal de operadores en Consorcio Nacional de Seguros, se actualiza a **MeteorJS** desde **PHP - MYSQL - JS - BOOTSTRAP** como tiene caracter de experimental no se recomienda su uso en produccion hasta la version 1, la cual se estima que va a ser publicada en 2 meses despues de todas las pruebas practicas.

version anterior [Portal Bitacora V1](https://github.com/kojimairiguchi/portalBitacora)
## Tabla de Contenidos
+ [Personal Involucrado](#Peronal Involucrado)
+ [Equipo](#Equipo)
+ [Estructura](#Estructura)
  + [Interna](#Interna)
  + [Externa / Publica](#Externa)
+ [Packages](#Packages)
+ [Notas](#Notas)

### Personal Involucrado
como beta test van a estar operadores de Consorcio Nacional de Seguros, supervisados por Nicolas Martinez

en el desarrollo van a estar [Nicolas Martinez](https://github.com/kojimairiguchi) ,  consultado por Salvador Maureira Briones

### Equipo
El equipo que se utiliza para esta es una maquina virtual con CentOS 6.5

### Estructura
#### Interna
la Estructura del sitio internamente va a ser así
```
+ client
  + templates
    + home.html
    + notas.html
    + entradas.html
    + exportar.html
    + busqueda.html
  + administracion
    + index.html
    + operaciones.html
  + sections
    + header.html
    + navbar.html
    + layouts
      + mainlayout.html
      + adminlayout.html
  + script
    + scripts.js
+ server
+ lib
  + routes.js
+ bases
+ index.html

```

mas información disponible en la ruta `lib/routes.js`

#### Publica

### Packages

los packages utlizados en esta version son:
```
# Meteor packages used by this project, one per line.
# Check this file (and the other files in this directory) into your repository.
#
# 'meteor add' and 'meteor remove' will edit this file for you,
# but you can also edit it by hand.

meteor-base             # Packages every Meteor app needs to have
mobile-experience       # Packages for a great mobile UX
mongo                   # The database Meteor supports right now
blaze-html-templates    # Compile .html files into Meteor Blaze views
session                 # Client-side reactive dictionary for your app
jquery                  # Helpful client-side library
tracker                 # Meteor's client-side reactive programming library

standard-minifiers      # JS/CSS minifiers run for production mode
es5-shim                # ECMAScript 5 compatibility for older browsers.
ecmascript              # Enable ECMAScript2015+ syntax in app code



kadira:flow-router
kadira:blaze-layout
erasaur:meteor-lodash
fortawesome:fontawesome
spiderable
fastclick
raix:handlebar-helpers
aldeed:collection2
aldeed:autoform
accounts-ui
accounts-password
matb33:bootstrap-glyphicons
zimme:active-route
gwendall:auth-client-callbacks
meteortoys:allthings
bootswatch:superhero
numtel:mysql
hitchcott:qr-scanner
aslagle:reactive-table

```

se preeve priscender de mongoDB en versiones futuras


### notas
- se van a hacen las pruebas usando los perfiles de usuario ``test``, ``test@test.cl``  y password ``1234``
- la base de datos va a estar pre-poblada y disponible en `sql/base.sql`
