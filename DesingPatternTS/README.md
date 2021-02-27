# Design Patterns in TypeScript

This repository is part of the [Refactoring.Guru](https://refactoring.guru/design-patterns) project.

It contains TypeScript examples for all classic GoF design patterns. Each pattern includes two examples:

- [x] **Conceptual** examples show the internal structure of patterns, including detailed comments.

- [ ] **RealWorld** examples show how patterns can be used in real-world web applications.

## Requirements

For simplicity reasons, the examples are console apps. In order to launch them, you have to install [Node.js and NPM](https://nodejs.org/en/) on your computer and then install [TypeScript compiler](https://github.com/Microsoft/TypeScript) and [TypeScript Node extension](https://github.com/TypeStrong/ts-node) like this:

```
npm install -g typescript
npm install -g ts-node
```

When you have all the required software installed, the examples can be launched via the command line as follows:

```
ts-node src/Path-to-example/Example.ts
```

For the best experience, I recommend working with examples with these IDEs:

- [WebStorm](https://www.jetbrains.com/webstorm/)
- [Visual Studio Code](https://code.visualstudio.com/)


## Contributor's Guide

I appreciate any help, whether it's a simple fix of a typo or a whole new example. Just [make a fork](https://help.github.com/articles/fork-a-repo/), make your change and submit a [pull request](https://help.github.com/articles/creating-a-pull-request-from-a-fork/).

Here's a style guide which might help you to keep your changes consistent with the rest of the project's code:

1. All code should follow these two guidelines: [Unofficial TypeScript StyleGuide](https://github.com/basarat/typescript-book/blob/master/docs/styleguide/styleguide.md) and [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript).

2. Try to hard wrap the code at 80th's character. It helps to list the code on the website without scrollbars.

3. Example files should be located and named in the following manner:

    ```
    src/{PatternName}/{ExampleName}/index.ts
    ```

4. Aim to put all code within one file. Yes, I realize that it's not how it supposed to be done in production. But it helps people to better understand examples, since all code fits into one screen.

5. Comments may or may not have language tags in them, such as this:

    ```typescript
    /**
     * EN: All products families have the same varieties (MacOS/Windows).
     *
     * This is a MacOS variant of a button.
     *
     * RU: Все семейства продуктов имеют одни и те же вариации (MacOS/Windows).
     *
     * Это вариант кнопки под MacOS.
     */
    ```

    This notation helps to keep the code in one place while allowing the website to generates separate versions of examples for all listed languages. Don't be scared and ignore the non-English part of such comments. If you want to change something in a comment like this, just do it. Even if you do it wrong, we'll tell you how to fix it during the Pull Request.


## License

This work is licensed under a Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/80x15.png" /></a>


## Credits

Authors: Alexey Pyltsyn ([@lex111](https://github.com/lex111)) and Alexander Shvets ([@neochief](https://github.com/neochief))




# Creational Patterns
  ## Abstract Factory

Creates an instance of several families of classes

Permite producir familias de objetos relacionados sin especificar sus clases concretas.


![](imagen/python/abstract-factory-mini.png)  ![](imagen/javascript/javascript-abstract-factory.jpg)

  ## Builder

Separates object construction from its representation

Permite construir objetos complejos paso a paso. Este patrón nos permite producir distintos tipos y representaciones de un objeto empleando el mismo código de construcción.

![](imagen/python/builder-mini.png)  ![](imagen/javascript/javascript-builder.jpg)

  ## Factory Method

Creates an instance of several derived classes

Proporciona una interfaz para la creación de objetos en una superclase, mientras permite a las subclases alterar el tipo de objetos que se crearán.

![](imagen/python/factory-method-mini.png)  ![](imagen/javascript/javascript-factory-method.jpg)

  ## Prototype

A fully initialized instance to be copied or cloned

Permite copiar objetos existentes sin que el código dependa de sus clases.

![](imagen/python/prototype-mini.png)  ![](imagen/javascript/javascript-prototype.jpg)

  ## Singleton

A class of which only a single instance can exist

Permite asegurarnos de que una clase tenga una única instancia, a la vez que proporciona un punto de acceso global a dicha instancia.

![](imagen/python/singleton-mini.png)  ![](imagen/javascript/javascript-singleton.jpg)

# Structural Patterns
  
  ## Adapter

Match interfaces of different classes

Permite la colaboración entre objetos con interfaces incompatibles.

![](imagen/python/adapter-mini.png)  ![](imagen/javascript/javascript-adapter.jpg)

  ## Bridge

Separates an object’s interface from its implementation

Permite dividir una clase grande o un grupo de clases estrechamente relacionadas, en dos jerarquías separadas (abstracción e implementación) que pueden desarrollarse independientemente la una de la otra.

![](imagen/python/bridge-mini.png)  ![](imagen/javascript/javascript-bridge.jpg)

  ## Composite

A tree structure of simple and composite objects

Permite componer objetos en estructuras de árbol y trabajar con esas estructuras como si fueran objetos individuales.

![](imagen/python/composite-mini.png)  ![](imagen/javascript/javascript-composite.jpg)

  ## Decorator

Add responsibilities to objects dynamically

Permite añadir funcionalidades a objetos colocando estos objetos dentro de objetos encapsuladores especiales que contienen estas funcionalidades.

![](imagen/python/decorator-mini.png)  ![](imagen/javascript/javascript-decorator.jpg)

  ## Facade

A single class that represents an entire subsystem

Proporciona una interfaz simplificada a una biblioteca, un framework o cualquier otro grupo complejo de clases.

![](imagen/python/facade-mini.png)  ![](imagen/javascript/javascript-facade.jpg)

  ## Flyweight

A fine-grained instance used for efficient sharing

Permite mantener más objetos dentro de la cantidad disponible de memoria RAM compartiendo las partes comunes del estado entre varios objetos en lugar de mantener toda la información en cada objeto.

![](imagen/python/flyweight-mini.png)  ![](imagen/javascript/javascript-flyweight.jpg)

  ## Proxy

An object representing another object

Permite proporcionar un sustituto o marcador de posición para otro objeto. Un proxy controla el acceso al objeto original, permitiéndote hacer algo antes o después de que la solicitud llegue al objeto original.

![](imagen/python/proxy-mini.png)  ![](imagen/javascript/javascript-proxy.jpg)


# Behavioral Patterns

  ## Chain of Responsibility

A way of passing a request between a chain of objects

Permite pasar solicitudes a lo largo de una cadena de manejadores. Al recibir una solicitud, cada manejador decide si la procesa o si la pasa al siguiente manejador de la cadena.

![](imagen/python/chain-of-responsibility-mini.png)  ![](imagen/javascript/javascript-chain-of-responsibility.jpg)

  ## Command

Encapsulate a command request as an object

Convierte una solicitud en un objeto independiente que contiene toda la información sobre la solicitud. Esta transformación te permite parametrizar los métodos con diferentes solicitudes, retrasar o poner en cola la ejecución de una solicitud y soportar operaciones que no se pueden realizar.

![](imagen/python/command-mini.png)  ![](imagen/javascript/javascript-command.jpg)

  ## Interpreter

A way to include language elements in a program

![](imagen/javascript/javascript-interpreter.jpg)

  ## Iterator

Sequentially access the elements of a collection

Permite recorrer elementos de una colección sin exponer su representación subyacente (lista, pila, árbol, etc.).

![](imagen/python/iterator-mini.png)  ![](imagen/javascript/javascript-iterator.jpg)

  ## Mediator

Defines simplified communication between classes

Permite reducir las dependencias caóticas entre objetos. El patrón restringe las comunicaciones directas entre los objetos, forzándolos a colaborar únicamente a través de un objeto mediador.

![](imagen/python/mediator-mini.png)  ![](imagen/javascript/javascript-mediator.jpg)

  ## Memento

Capture and restore an object's internal state

Permite guardar y restaurar el estado previo de un objeto sin revelar los detalles de su implementación.

![](imagen/python/memento-mini.png)  ![](imagen/javascript/javascript-memento.jpg)

  ## Observer

A way of notifying change to a number of classes

Permite definir un mecanismo de suscripción para notificar a varios objetos sobre cualquier evento que le suceda al objeto que están observando.

![](imagen/python/observer-mini.png)  ![](imagen/javascript/javascript-observer.jpg)

  ## State

Alter an object's behavior when its state changes

Permite a un objeto alterar su comportamiento cuando su estado interno cambia. Parece como si el objeto cambiara su clase.

![](imagen/python/state-mini.png)  ![](imagen/javascript/javascript-state.jpg)

  ## Strategy

Encapsulates an algorithm inside a class

Permite definir una familia de algoritmos, colocar cada uno de ellos en una clase separada y hacer sus objetos intercambiables.

![](imagen/python/strategy-mini.png)  ![](imagen/javascript/javascript-strategy.jpg)

  ## Template Method

Defer the exact steps of an algorithm to a subclass

Define el esqueleto de un algoritmo en la superclase pero permite que las subclases sobrescriban pasos del algoritmo sin cambiar su estructura.

![](imagen/python/template-method-mini.png)  ![](imagen/javascript/javascript-template-method.jpg)

  ## Visitor

Defines a new operation to a class without change

Permite separar algoritmos de los objetos sobre los que operan.

![](imagen/python/visitor-mini.png)  ![](imagen/javascript/javascript-visitor.jpg)
