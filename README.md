Aplicativo criado com React Native Navigation Stack

1. Instalando o Expo
A instalação do Expo no computador é feita pelo Node através do comando:
npm install -g expo-cli

2.  Comando para se logar em uma conta expo:
expo login

3. Criar o projeto
Entrar na pasta que o projeto será criado através do cmd ou terminal do vscode e digitar o comando:
npx create-react-native-app <nome do projeto>

4. Instalar as bibliotecas através do npm do node.js:
npm install @react-navigation/native @react-navigation/stack

npx expo install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view

5. Babel.config.js

module.exports = function(api) {
  api.cache(true);
  return {
    presets: ['babel-preset-expo'],
    plugins: ['react-native-reanimated/plugin'],
  };
};

6. Executar o aplicativo através do comando:
npx expo start

7. Gerar o instalador .apk ou .aab (android):
expo build:android

8. Gerar o instalador .ipa (ios):
expo build:ios

