#Rails Stimulus Generator
A simple rails generator to help generate new Stimulus controllers.

to download, go to your rails project root and run

```
curl
```

then you can generate new controllers by running

```
rails g stimulus controller_name
```

and that will generate for you a new controller at

```
app/javascript/controllers/name_controller.js
```

with the file contents

```
import { Controller } from "stimulus";

export default class extends Controller {
  static targets = [];

  initialize() {
    // Called once, when the controller is first instantiated
  }

  connect() {
    // Called any time the controller is connected to the DOM
  }

  disconnect() {
    // Called any time the controller is disconnected from the DOM
  }
}
```
