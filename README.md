# es6-eslint-app

This app contains the pre configuration setup for ES6 + ESLINT
<br/>

<b># STEP 1</b><br/>
<u>ES6</u><br/>
npm install --save-dev @babel/node @babel/core @babel/cli @babel/preset-env @babel/preset-typescript<br/>
create .babelrc in the root folder and paste the code<br/>
<code>
{
"presets": ["@babel/env", "@babel/typescript"]
}
</code><br/>

<b># STEP 2</b><br/>
<u>ESLINT</u><br/>
For more info - https://blog.echobind.com/integrating-prettier-eslint-airbnb-style-guide-in-vscode-47f07b5d7d6a<br/>
npm install -D eslint prettier<br/>
npx install-peerdeps --dev eslint-config-airbnb<br/>
npm install -D eslint-config-prettier eslint-plugin-prettier<br/>
create .eslintrc in the root folder and paste the code<br/>
<code>
{
"extends": ["airbnb", "prettier"],
"plugins": ["prettier"],
"rules": {
"prettier/prettier": ["error"]
}
}
</code><br/>
create .prettierrc in the root folder and paste the code<br/>
<code>
{
"printWidth": 100,
"singleQuote": true
}
</code><br/>
