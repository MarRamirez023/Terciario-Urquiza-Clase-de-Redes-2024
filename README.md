# Terciario-Urquiza-Clase-de-Redes-2024
Practica de la clase de redes y comunicación del terciario Urquiza

# Primer nivel de encabezado
## segundo nivel de encabezado
### Tercer nivel de encabezado
#### Cuarto nivel de ancabezado

Lista de compras

* Frutas
 * Manzanas
 * Naranjas
 * Uvas

* Lacteos
 * Leche
 * Queso

Lista de pendientes

1. Terminar el tutorial de Markdown
2. Ir a la tienda de abarrotes
3. Preparar el almuerzo

```html
<html>
	<head>
    	<title>Título del sitio Web</title>
	</head>
	<body>
	</body>
</html>
```

|Encabezado 1|Encabezado 2|Encabezado 3|
|---------|---------|---------|
|Reglon 1, Columna 1|Reglon 1, Columna 2|Reglon 1, Columna 3|
|Reglon 2, Columna 1|Reglon 2, Columna 2|Reglon 2, Columna 3|
|Reglon 3, Columna 1|Reglon 3, Columna 2|Reglon 3, Columna 3|

```mermaid
classDiagram
    class Libro {
        +String titulo
        +String autores
        +String isbn
        +boolean isAvailable()
    }

    class Member {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }

    class Librarian {
        +String name
        +String employeeId
        +addBook(Book book)
        +removeBook(Book book)
    }

    class Library {
        +String name
        +List<Book> books
        +List<Member> members
        +List<Librarian> librarians
        +addMember(Member member)
        +removeMember(Member member)
    }

    Libro --> Library : contiene
    Member --> Library : registra
    Librarian --> Library : administra
