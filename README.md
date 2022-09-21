Aplicativo criado com React Native Navigation Drawer

1. Instalando o Expo
A instalação do Expo no computador é feita pelo Node através do comando:
npm install -g expo-cli

2. Criar o projeto
Entrar na pasta que o projeto será criado através do cmd ou terminal do vscode e digitar o comando:
npx create-react-native-app <nome do projeto>

3. Instalar as bibliotecas através do npm do node.js:
npm install @react-navigation/native @react-navigation/stack

npx expo install react-native-gesture-handler react-native-reanimated react-native-screens react-native-safe-area-context @react-native-community/masked-view

4. Babel.config.js

module.exports = function(api) {
  api.cache(true);
  return {
    presets: ['babel-preset-expo'],
    plugins: ['react-native-reanimated/plugin'],
  };
};

5. Executar o aplicativo através do comando:
npx expo start

6.  Comando para se logar em uma conta expo
expo login

7. Comando para instalar uma ferramenta responsável por gerar o instalador do Android 
npm install -g eas-cli

8.Comando para se gerar um .apk ou .aab
eas build -p android

