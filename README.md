criado apenas para entender como instala e funciona essa ferramenta(presets)
Presets em JavaScript (JS) são conjuntos de configurações ou funções pré-definidas que facilitam a aplicação de estilos, transformações ou comportamentos complexos de forma rápida e consistente, como coleções de plugins para o Babel, que aplicam transformações de código de uma vez, ou estilos visuais para imagens, que agrupam ajustes de cor e luz para serem aplicados em lote, economizando tempo e garantindo um padrão visual. 

Em Contexto de Desenvolvimento (Ex: Babel, Webpack):
• O que são: São grupos de configurações ou plugins que um bundler ou transpiler (como o Babel) usa para processar código JavaScript.
• Para que servem: Permitem que você use recursos modernos do JS (como ES6+) e eles são automaticamente convertidos para uma versão compatível com navegadores mais antigos, aplicando várias transformações (plugins) de uma só vez.
Exemplo: @babel/preset-env é um preset que transforma o JavaScript moderno para que funcione em diversos ambientes, sem que você precise configurar cada plugin de transformação individualmente

============================================================================= Usando o Babel ==========================================================================================================

Com o carregamento do bandle, todos os sites consiguirtam ler os scripts, pois ele sera convertido para o modo antigo
para ser usado o babel, é so ir no terminal e digitar...

Instalação:
npm install --save-dev @babel/cli @babel/preset env @babel/core

pos os arquivos de scriptrs pronto ´e so usaro babel q sera criado um arquivo novo chamado BUDLE.JS esse arquivo sera o arquivo q ira carregar posteriormente
Conversao:
npx babel nomedoarquivo -o bundle.js --presets=@babel/env

Para q essa conversao seja feita de forma automaticamente:
1- vá no packge.json
2- vá em "scripts": { "test": "echo \"Error: no test specified\" && exit 1",
"converção": babel ./main.js -o./bungle.js --presets=@babel/env -w

Para executar:
npm run babel
aq ele executara sem parar, aq ele esta assistindo tudo q esta sendo feito
