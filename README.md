## Elm is a programming language that compiles to JavaScript.

#### The highlight features are great performance:
 - No runtime errors in practice. No null. No undefined is not a function.
 - Friendly error messages that help you add features more quickly.

    ![alt](http://elm-lang.org/assets/blog/error-messages/0.16/expected-arg.png)

 - Well-architected code that stays  well-architected as your app grows.   
 - Automatically enforced semantic versioning for all Elm packages.

#### How to install :
 ```js
 sudo npm install -g elm
 ```
#### To install elm-package.json:
 ```js
 elm-package install
 ```
#### The Basic Pattern :
 - Model — the state of your application
 - Update — a way to update your state
 - View — a way to view your state as HTML

```js
import Html exposing (..)


-- MODEL

type alias Model = { ... }


-- UPDATE

type Msg = Reset | ...

update : Msg -> Model -> Model
update msg model =
  case msg of
    Reset -> ...
    ...


-- VIEW

view : Model -> Html Msg
view model =
  ...
```

#### To run this example:
```js
elm-reactor
```

This starts a server at
 http://localhost:8000,
then type

http://localhost:8000/main.html
