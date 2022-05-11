## Пакет DebugModels для lumen микросервисов

### Установка пакета
- ```composer require sixsad/debug-models```

Для работы пакета необходимо создать папку `config` в микросервисе и добавить следующий код: 
```php
<?php

return [

    "include" => (bool)env("DEBUG_MODELS_INCLUDE", false),
    "debugDir" => env("DEBUG_MODELS_ROOT", 'app/DebugModels/'),

];
```
