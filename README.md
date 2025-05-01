# Tabla de Contenidos

- [Tabla de Contenidos](#tabla-de-contenidos)
- [React Native](#react-native)
  - [¿Qué es?](#qué-es)
  - [Aplicaciones que usan Native](#aplicaciones-que-usan-native)
  - [Ventajas de Native](#ventajas-de-native)
  - [Desventajas de Native](#desventajas-de-native)
  - [Recursos](#recursos)
- [Native para Móvil](#native-para-móvil)
  - [Expo como Framework](#expo-como-framework)
  - [Crear Proyecto](#crear-proyecto)
    - [Sobre previsualización en Móvil](#sobre-previsualización-en-móvil)
  - [Estructura del Proyecto](#estructura-del-proyecto)
- [Native para Escritorio](#native-para-escritorio)

# React Native

## ¿Qué es?

React Native (Native de ahora en más) es un plataforma de desarrollo creada para poder desarrollar aplicaciones móviles, web y de escritorio creada por meta en 2015 basada en React, usa la misma biblioteca.

La diferencia principal entre React y Native radica en que para renderizar React en web usamos la libreria `react-dom` que no está presente en Native (no tenemos un DOM en escritorio/móvil).

Native usa código nativo que hace de puente para que nosotros escribamos JavaScript (JS) o TypeScript (TS) y esto se comunique con el sistema. La diferencia entre Native con Ionic o Electron es que esto es una página web empaquetada mientras que Native usa código nativo.

En el caso de las aplicaciones de escritorio es necesario usar `react-native-window` o `react-native-macos` ambas desarrolladas por Microsoft que permiten llevar nuestro código a ambos Sistemas Operativos (OS).

## Aplicaciones que usan Native

En el caso de aplicaciones móviles tenemos ejemplos como Facebook, Xbox GamePass, Microsoft Office, Microsoft Teams, Discord, Pinterest, entre muchas más; mietras que en escritorio tenemos casos como el de Microsoft Office y la aplicación de Xbox.

## Ventajas de Native

La más evidente es que permite tener un solo código para que una aplicación llegue a muchas plataformas.

No obstante también tenemos que es bastante demandado, bastante más que Ionic; es simple de usar, otorga un fast refresh para ver los cambios sin necesidad de compilar, posee una gran comunidad y que su rendimiento es mucho mejor a otras alternativas (como Ionic o Electron).

Otra ventaja, y una muy importante, es lo sencillo que es hacer actualizaciones OTA (Over The Air), es decir, actualizaciones que no tengan que pasar por la tienda de aplicaciones.

## Desventajas de Native

En primer lugar está el rendimiento, aunque no es malo y en general está bastante bien, cualquiera que haya usado alguna de las aplicaciones que mencioné puede comprobarlo; nunca va a ser tan eficiente en rendimiento como una aplicación completamente nativa.

Por otro lado está que nunca vamos a tener las novedades del SO en el momento de su salida, por ejemplo, es probable que cuando Apple lance su IA a los IPhones de una API para que los desarrolladores de Swift puedan utilizarla, pero si nosotro trabajamos con Native tendremos que esperar a que alguien cree el módulo nativo (o crearlo nosotros mismos).

Por último tenemos la dependencia de componentes de terceros, es probable que cuando queramos hacer algo nos encontremos con que Native no tiene una forma de hacerlo pero que alguien ya se encontró ese problema y creó un componente para solucionarlo, hay personas que podían encontrar inconveniente o molesto tener que buscar estas soluciones.

## Recursos

- Documentación ([docs](https://reactnative.dev/))
- Introducción a React Native por MiduDev ([video](https://www.youtube.com/watch?v=U23lNFm_J70))


# Native para Móvil

## Expo como Framework

Native por si sólo está muy centrado en manejar la UI pero ciertas funcionalidades, como el enrutado o usar el Bluethoot y la cámara, que no están directamente en la librería. Es aquí donde entra Expo como el encargado de agregar todo esto.

Expo no es una recomendación personal, es la que recomienda el propio equipo de Native.

## Crear Proyecto

Al igual que pasa con tencologias como Electron, Expo y React Native tienen problemas con `pnpm`, por lo que se recomienda usar `npm` o `yarn`. Para crear un poryecto de Expo usamos el siguiente comando:

```sh
npx create-expo-app
```

O en caso de querer utilizar Yarn

```sh
yarn dlx create-expo-app
```

A continuación Expo nos pedirá que le demos un nombre al proyecto.

Esto creará un proyecto por defecto con algunas facilidades como poder rápidamente ver nuestro proyecto con Android SDK, fast refresh y una serie de herramientas de desarrollo.

### Sobre previsualización en Móvil

Es posible previsualizar nuestra aplicación de 4 formas distintas para cada OS (Android y IOS), podemos hacerlo en un dispositivo o por medio de un emulador/simulador y a través de Expo Go o un Build de desarrollo. La explicación de cómo configurar cada una es extensa por lo que no la pondré aquí esta se puede ver en la [documentacion](https://docs.expo.dev/get-started/set-up-your-environment/).

Algo que si es necesario aclarar es que para previsualizar nuestr app en IOS necesitaremos un dispositivo de Apple, ya sea un Mac o un IPhone, esto porque no existen emuladores de IOS para Windows, por lo menos no confiables.

## Estructura del Proyecto

> [!WARNING]
> IN PROGRESS...

# Native para Escritorio

> [!WARNING]
> IN PROGRESS...
