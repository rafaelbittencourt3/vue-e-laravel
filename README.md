# Vuejs-e-laravel
Configurações Iniciais Vue e Laravel

1#
Instale o Vue.js: você pode fazer isso com um gerenciador de pacotes, como o NPM.
Execute o seguinte comando no terminal:
```sh
npm install vue
```
2#
Crie um arquivo app.js em sua pasta de recursos js:
```sh
/resources/js/app.js
```
3#
Adicione o seguinte código em seu arquivo app.js:

```sh

import Vue from 'vue';
import ExampleComponent from './components/ExampleComponent.vue';

Vue.component('example-component', ExampleComponent);

const app = new Vue({
  el: '#app',
});

```

4# Crie um arquivo blade em sua pasta de recursos views:
```sh
/resources/views/welcome.blade.php
```
5# Adicione o seguinte código ao seu arquivo blade:
```sh
<html>
  <head>
    <title>My App</title>
  </head>
  <body>
    <div id="app">
      <example-component></example-component>
    </div>
    <script src="{{ mix('js/app.js') }}"></script>
  </body>
</html>
```
6# Compile seu arquivo app.js usando o comando do Laravel Mix:
```sh
npm run dev
```
7# Abra o arquivo welcome.blade.php no navegador e verifique se o componente ExampleComponent do Vue.js foi renderizado corretamente.

Estas são as etapas básicas para configurar app.js com Vue.js em uma aplicação Laravel. No entanto, é importante lembrar que a configuração exata pode variar dependendo da versão do Laravel e do Vue.js que você está usando. Certifique-se de ler a documentação do Laravel e do Vue.js para obter instruções mais detalhadas e precisas.
