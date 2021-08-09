# Development GuideLines Weepec

## Tecnologias
* Frontend
    * Reactjs
    * ReactNative
    * Nodejs
    * Vuejs
    * MongoDB
* Server
    * Docker
    * Docker-Compose
* Backend
    * Prisma
    * Graphql
    * Loopback4
* Storage
    * Redis
    * Redux
    * MongoDB

## Creación de repositorio 
Se debe tener una notaciòn en la cual se denote 3 partes
* Proyecto al cual se pertenece (weepec)
* Ambito
* tecnologia principal

```
[Proyecto]-[Ambito]-[Tecnologia]
```

el cual quedaria como 

```
weepec-app-reactnative
```
## Manejo de ramas

Este debe ser con el flujo de trabajo git-flow, se deja una pequeña referencia [aquí](https://www.atlassian.com/es/git/tutorials/comparing-workflows/gitflow-workflow)

## Commits a repositorios

Motivación: 
You might say, "It's just a personal project." Yes, you work alone now, but what happens when you work with a team or contribute to open source?

A well-crafted Git commit message is the best way to communicate context about a change to other developers working on that project, and indeed, to your future self.

Have you ever tried running git log on one of your old projects to see the "weird" commit messages you have used since its inception? It can be hard to understand why you made some changes in the past, and you'll wish you read this article earlier :)

Commit messages can adequately communicate why a change was made, and understanding that makes development and collaboration more efficien

```text
Capitalized, short (50 chars or less) summary

More detailed explanatory text, if necessary.  Wrap it to about 72
characters or so.  In some contexts, the first line is treated as the
subject of an email and the rest of the text as the body.  The blank
line separating the summary from the body is critical (unless you omit
the body entirely); tools like rebase can get confused if you run the
two together.

Write your commit message in the imperative: "Fix bug" and not "Fixed bug"
or "Fixes bug."  This convention matches up with commit messages generated
by commands like git merge and git revert.

Further paragraphs come after blank lines.

- Bullet points are okay, too

- Typically a hyphen or asterisk is used for the bullet, followed by a
  single space, with blank lines in between, but conventions vary here

- Use a hanging indent

If you use an issue tracker, add a reference(s) to them at the bottom,
like so:

Resolves: #123
```

1. Especificar tipo de commit
    * `feat`: The new feature you're adding to a particular application
    * `fix`: A bug fix
    * `style`: Feature and updates related to styling
    * `refactor`: Refactoring a specific section of the codebase
    * `test`: Everything related to testing
    * `docs`: Everything related to documentation
    * `chore`: Regular code maintenance.[ You can also use emojis to represent commit types]

The symbol ”!” can be used with any type. It signifies a breaking change that correlates with MAJOR in semantic versioning.
Using BREAKING CHANGE in the footer introduces a breaking API change as well (correlating with MAJOR in semantic versioning).

2. Separate the subject from the body with a blank line
3. Your commit message should not contain any whitespace errors
4. Remove unnecessary punctuation marks
5. Do not end the subject line with a period
6. Capitalize the subject line and each paragraph
7. Use the imperative mood in the subject line
8. Use the body to explain what changes you have made and why you made them.
9. Do not assume the reviewer understands what the original problem was, ensure you add it.
10. Do not think your code is self-explanatory
11. Follow the commit convention defined by your team

# Revisión de código 
## Puntos a considerar
* Evitar código comentado en cualquier punto
* uso de `console.log` debe de ser unicamente en desarrolo y cierto punto de debuging
* no usar segmentación de código y repetir código
