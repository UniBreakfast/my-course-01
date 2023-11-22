# 5 levels to think on for a programmer

## [Русский](five-levels.ru.md) | English | [Українська](five-levels.ua.md)

Programming in the context of the web and JavaScript is somewhat more complicated than just writing code. It requires thoughtful organization of projects, data and interaction systems. In this article we will consider five main levels of thinking that a programmer should differentiate in order for his reasoning not to turn into a mess, and projects - into balls of incomprehensible coddity.

---

### 1st level. Folders and Files

At this level, we are talking about structuring the project at the physical level. How best to organize **folders and files** of the project so that the code is readable and easy to maintain? You can write everything in one file, you can divide **by languages** (.html, .css, .js), **by purpose** - putting components in separate files or even folders, **by sides** of client-server interaction - Front/Backend. Or even apply a more detailed methodology (7-1, etc.).

Adequate organization of code into different files and folders helps to separate responsibilities and simplifies navigation through the project. Moreover, in development there may be one division into files and in the application deployed on the server - another, organized using a project builder (Webpack, Parcel, Rollup, etc.).

At this level we decide where to write. On the next - what we write.

### 2nd level. Code: Statements, Expressions, Tokens

At the code level, the program turns from abstract ideas into specific commands, written in accordance with the **syntax** - a set of requirements for the code that must be met.

When composing commands, it is important to distinguish statements from expressions. **Statements** are executed solely for their effect - imports, declarations, branching, loops, error traps and others. **Expressions** must return values, which ensures their high combinability into even more complex expressions. Based on the operators used, arithmetic and logical expressions, assignment, comparison, selection, access, call and others are distinguished.

It is also important to understand that any code (its statements and expressions) consists of **tokens** - atomic lexical units. In HTML, these are **tags, attributes with values and text**. In CSS, these are **directives, selectors, combinators and rule blocks with properties and values**.

And in JavaScript these are keywords, identifiers, operators, literals, punctuation and comments. **Keywords** should not be used for anything other than their intended purpose (most often in the corresponding statements). **Identifiers** identify (name) entities and should not be in conflict within one scope. **Operators** perform operations on data according to the order of writing, grouping and priority of execution. **Literals** literally create values. **Punctuation** separates other tokens where syntax requires it. **Comments** do not affect the execution of the code, but help to understand its meaning both to the programmer and to modern editors with intellisense and autocompletion.

### 3rd level. Data (values) and Data Structures

Decisions about choosing types and data structures and ways of organizing them are critically important for the developer. In JS, we have access to primitive (singular) values: **numbers** or **strings**, **boolean values** or **nullish**. Collections (complex): **arrays** (with numbered values in cells) or **objects** (with named values in properties). By choosing objects, we work with an assortment of hundreds of object types, standard for browsers or NodeJS.

Different types can be operated on with different complexity, execution speed and memory usage. Specific data structures from computer science can also be used: **hash tables, dictionaries, maps, trees, graphs, sets, lists, stacks, queues**... - each with its own advantages and disadvantages.

At this level we decide how and what data we store. On the next - how we work with it.

### 4th level. Entities that operate on data

It is important to keep in mind that without being tied to entities, the created data is almost immediately destroyed by the garbage collector to free up memory. To avoid this, it is necessary to link values to entities that provide access to them and the ability to manipulate them. These are variables, constants, parameters and properties for storing data and accessing it, as well as functions, methods and classes for creation and multi-step operations on them.

**Variables and constants** are named references to data. **Functions** are anonymous or named blocks of code that can be called however many times their execution is required. **Parameters** are named references to values passed to a function (**arguments**). **Properties** are references to data belonging to an object, named uniquely within it with **keys**. Array cells, numbered by indexes, actually are also object properties (and indexes are their keys). **Methods** are functions belonging to an object. **Constructor functions or Classes** are templates for creating typical objects (instances).

It is important to understand that variables and constants do not store data in themselves (although we will continue to think of them in this way, because it is easier and more convenient for us) - only references to them.

### 5th level. Interfaces: GUI, CLI, API

The last level of thinking is related to interfaces.

**Graphical User Interface** (GUI) is a composition of all those elements on the screen through which information is shown to users, and by means of which they interact with the application (forms, input fields, buttons, links, state switches). Accessibility and understanding of the principles of User Experience (UX) are important here.

**Command Line Interface** (CLI) is a chat-like interface through which the user interacts with the application through text commands. It is not so visual and convenient, but it can be automated easily.

**Application Programming Interface** (API) is a programmatic interface of the application, according to which subprograms and entire applications interact with each other in a coordinated manner, forming complex systems with even wider capabilities.

---

Choosing and implementing optimal solutions at each of these levels is the key to successful development. This not only helps to create efficient and reliable software solutions, but also makes the process understandable and manageable. **Try to form a clear idea of each of these five levels and test yourself by writing or saying your understanding**. This will help you make informed decisions and act on each of them. After all, ***the beauty of a project is in the obvious expediency of all its components***.

![abstract illustration](five-layers.jpg)
