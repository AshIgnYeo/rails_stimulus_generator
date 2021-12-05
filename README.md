# Rails Stimulus Generator

A simple rails generator to help generate new Stimulus controllers.

Before anything, ensure you have stimulus by running

```
rails webpacker:install:stimulus
```

Once you have stimulus in your project, go to your rails project root and run

```
mkdir lib/generators && cd $_
curl -L -O https://github.com/AshIgnYeo/rails_stimulus_generator/raw/master/stimulus.zip
unzip -q stimulus.zip && rm -rf stimulus.zip __MACOSX
cd ../..
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
