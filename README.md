# Lerna without yarn workspaces

```
npm install lerna -g
```

:thinking: I'd like to install this non-globally, but then: how would I use lerna inside of a package in this repo?


## Gotchas
Cannot have @org name in the root/package.json 

:angry: Bad
```
// root package.json

name: "@myorg/root"
```

:rocket: Good
```
// root package.json

name: "myorg"
```

## Adding a peer dependency to a package


```
lerna add react packages/two --peer
```

## How to add package-lock to each package?!

```
lerna exec -- npm i
```

## Running the `app`

```
lerna run start
```