vue.js presentation

Vue.js is a framework built with JavaScript, focused on **building user interfaces**. It simplifies complex front-end development tasks like data binding, component-based development, and state management, and provides pre-packaged features and tools. This allows developers to build dynamic, interactive applications more quickly and efficiently without having to write extensive native JavaScript code.

![1](pictures/1.png)

The cover slide of the presentation, showing the team members and the selected topic.![2](pictures/2.png)

Here, we’ve included an agenda to give the audience an overview of the presentation flow.![3](pictures/3.png)

Next is the first section: Introduction.

![4](pictures/4.png)

Vue.js is actually a progressive JavaScript framework primarily used for building front-end user interfaces.

Its features are also quite distinct: simplicity, high efficiency, support for component-based development, two-way data binding, and other integrated functions.

![5](pictures/5.png)

Next, we’ll provide a simple demonstration to help unfamiliar viewers understand how to use this framework.

First, install the Vue CLI. Open the target folder in VS Code, create a new terminal, and enter the following command:![6](pictures/6.png)

`npm install -g @vue/cli`

This will globally install the Vue CLI.

![7](pictures/7.png)

Next, use the following command to create your own Vue.js project: `vue create my-vue-app`(replace *`my-vue-app`* with your preferred project name). Then, a prompt will appear, allowing you to choose the version of Vue you need. The latest version is Vue 3. If you’ve used an older version for previous projects and want to continue editing them, make sure to select the corresponding version for download. By default, the latest version is selected. If you’re a professional developer, you can select the last option to customize the version and layout settings.

![8](pictures/8.png)

After installation, you’ll see that the system has prompted you on how to run the project.

![9](pictures/9.png)

First, enter  `cd my-vue-project` (replace *`my-vue-app`* with the directory of your created project), and then enter npm run serve to officially run the project.

If you want to use related plugins, you can check and install them on GitHub; however, they’re unnecessary for simple examples.

![10](pictures/10.png)

Next is a detailed analysis of each part of the Vue.js framework.![11](C:\Users\27406\Desktop\vue.js\pictures\11.png)

This section mainly includes configuration files for the project, which beginners do not need to modify at all.

![12](pictures/12.png)

The *index.html* page is quite important, as Vue.js renders the entire application at this mounting point, defining the basic structure of the webpage.

![13](pictures/13.png)

This concludes the detailed explanation of the Vue.js framework. If you'd like to learn more, you can find additional resources on GitHub.

![14](pictures/14.png)

Next, we’ll present a simple example created by our team to demonstrate where each part of the code should be placed within this framework.

![15](pictures/15.png)

The basic HTML part can be placed directly in *App.vue*. CSS and JavaScript can either be included within it or stored in separate files.

![16](pictures/16.png)

After creating it, don’t forget to go to *main.js* to mount it; otherwise, the system will throw an error and won’t run.

![17](pictures/17.png)

Next, we have a small project our team created with Vue.js—a calculator for basic arithmetic operations.

![18](pictures/18.png)

I’ve organized the code into categories for easier management.

![19](pictures/19.png)

This part is the main section of the JavaScript code.

![20](pictures/20.png)

This is the CSS and rendering interface.

![21](pictures/21.png)

Finally, the most crucial step is to return to the *main.js* file to mount your project, allowing it to run successfully.

![22](pictures/22.png)

<video src="pictures\10月20日.mp4"></video>



![23](pictures/23.png)

Next is an analysis of the user groups and use cases.

![24](pictures/24.png)

Firstly, I think Vue.js is very beginner-friendly, with a structure that’s not overly complex, making it easy to get started. As shown in the left image, the usage rate of Vue.js continues to rise.

It’s also quite convenient for other user groups.

![25](pictures/25.png)

In reality, many use cases require extensive structure, real-time data updates, and project integration, which are key reasons why users choose Vue.js.![26](pictures/26.png)

Next, I will present the advantages and disadvantages of Vue.js. Like any technology, it has both strengths and weaknesses.

![27](pictures/27.png)

The advantages are evident; however, the corresponding drawbacks are also clear. As the project becomes more complex, the required performance of the device running it increases, and it does not support simultaneous multi-user online editing, which is a significant limitation.

![28](pictures/28.png)

That is the complete presentation.



Tutorial

In fact, when using the Vue.js framework, many editors are available, each with its own advantages. My top recommendation is Visual Studio Code, one of the most popular code editors today, which supports a wide range of extensions, such as Vue.js extensions, debugging, formatting, and more. Next is Sublime Text, a lightweight editor that supports Vue.js syntax highlighting and extensions, making it suitable for quick code editing. Another option is Atom, an open-source editor developed by GitHub that also supports Vue.js plugins and some custom features. There are many other editors, but I won’t list them all here.

To start writing Vue.js applications in VSCode, you’ll need to install Node.js, as Vue.js relies on this environment. You can download and install it from the official Node.js website (https://nodejs.org/en).

![31](pictures/31.png)

After installation, open PowerShell or Command Prompt and enter the following command to check if Node.js has been installed correctly

`node -v`

If the version information is displayed, the installation was successful. If the command is not recognized or Node cannot be found, it means Node.js was not installed correctly, or the path was not added to the system environment variables.

To check if it’s been added to the system environment variables, go to your desktop, select "This PC," right-click, and choose "Properties." Select "Advanced system settings," then "Environment Variables." In the "System Variables" section, locate "Path," select it, and either double-click or click "Edit." Then click "Browse." If installed on the C drive, the default location is `C:\Program Files\nodejs\`. If it’s elsewhere, you can manually find and paste the directory path. After that, click "OK" all the way through to save.

Once everything is set, restart your computer to apply the changes. After restarting, open PowerShell again and run `npm -v`. If the version information is displayed, the setup is complete. If not, you may need to uninstall and reinstall Node.js.

<img src="pictures\42.jpg" alt="42" style="zoom:33%;" />

![32](pictures/32.png)

![33](pictures/33.png)

![34](pictures/34.png)

![35](pictures/35.png)

![36](pictures/36.png)



After setting up, you can use the Vue CLI to quickly generate a Vue.js template. Start by creating a new folder—I'll name it `my-vue-project`—and open this folder in VSCode. Open a new terminal and enter the following command to install Vue CLI globally:

`npm install -g @vue/cli`

Next, create a new Vue.js project by typing:

`vue create vue-js`

Here, I chose `vue-js` as the project name. If you encounter a message in the terminal stating that the system prohibits script execution, run PowerShell as an administrator and enter the following command to check the current execution policy:

`Get-ExecutionPolicy`

If it displays `Restricted` or `RemoteSigned`, it means PowerShell doesn’t allow scripts to run by default. In this case, enter the following command:

`Set-ExecutionPolicy RemoteSigned -Scope CurrentUser`

This command allows PowerShell to run local scripts while requiring signatures for remote scripts, enhancing system security. After that, you can rerun the command:

`vue create vue-js`

This step defaults to Vue 3. If you have projects in older versions and want to continue with them, you can select the version accordingly. For this guide, we’ll proceed with the latest Vue 3.

![37](pictures/37.png)

![38](pictures/38.png)

![39](pictures/39.png)

The system will then guide you on how to run the project by executing a series of commands in the terminal.

Hold down **CTRL** and click the **Local** link provided in the terminal output to open and view the initial project page in your browser.

![40](pictures/40.png)

This is the default project running page. Next, let’s look at how to set up and run our group project, "Calculator," and explore its project structure.

![41](pictures/41.png)

The following is the content of `index.html`.

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Calculator</title>
    <link rel="stylesheet" href="./assets/styles.css" />
  </head>
  <body>
    <div id="app"></div>
  </body>
</html>


***The following is the content of `calculator.js` in the `assets` folder.***

`export const calculatorMethods = {`

 `appendNumber(number) {`

  `if (this.result === '0') {`

   `this.result = number;`

  `} else {`

   `this.result += number;`

  `}`

 `},`

 `chooseOperator(operator) {`

  `if (this.result !== '') {`

   `this.firstValue = this.result;`

   `this.operator = operator;`

   `this.result = '';`

  `}`

 `},`

 `calculate() {`

  `if (this.firstValue !== null && this.operator !== null && this.result !== '') {`

   `this.secondValue = this.result;`

   `const num1 = parseFloat(this.firstValue);`

   `const num2 = parseFloat(this.secondValue);`

   `switch (this.operator) {`

​    `case '+':`

​     `this.result = (num1 + num2).toString();`

​     `break;`

​    `case '-':`

​     `this.result = (num1 - num2).toString();`

​     `break;`

​    `case '*':`

​     `this.result = (num1 * num2).toString();`

​     `break;`

​    `case '/':`

​     `if (num2 !== 0) {`

​      `this.result = (num1 / num2).toString();`

​     `} else {`

​      `this.result = 'Error';`

​     `}`

​     `break;`

   `}`

   `this.firstValue = null;`

   `this.operator = null;`

   `this.secondValue = null;`

  `}`

 `},`

 `clear() {`

  `this.result = '0';`

  `this.firstValue = null;`

  `this.operator = null;`

  `this.secondValue = null;`

 `}`

`};`

***Next is the `styles.css` file.***

`.calculator {`

 `text-align: center;`

 `margin-top: 50px;`

`}`

`input {`

 `width: 200px;`

 `height: 50px;`

 `font-size: 24px;`

 `text-align: right;`

 `margin-bottom: 20px;`

`}`

`button {`

 `width: 50px;`

 `height: 50px;`

 `font-size: 20px;`

 `margin: 5px;`

 `cursor: pointer;`

`}`

`button:hover {`

 `background-color: #c5f48f;`

`}`

***Next is the `App.vue` file.***

<template>
  <div id="app" class="calculator">
    <h1>Calculator</h1>
    <input type="text" v-model="result" readonly />


    <div>
      <button @click="appendNumber('7')">7</button>
      <button @click="appendNumber('8')">8</button>
      <button @click="appendNumber('9')">9</button>
      <button @click="chooseOperator('/')">÷</button>
    </div>
    <div>
      <button @click="appendNumber('4')">4</button>
      <button @click="appendNumber('5')">5</button>
      <button @click="appendNumber('6')">6</button>
      <button @click="chooseOperator('*')">×</button>
    </div>
    <div>
      <button @click="appendNumber('1')">1</button>
      <button @click="appendNumber('2')">2</button>
      <button @click="appendNumber('3')">3</button>
      <button @click="chooseOperator('-')">-</button>
    </div>
    <div>
      <button @click="appendNumber('0')">0</button>
      <button @click="clear">C</button>
      <button @click="calculate">=</button>
      <button @click="chooseOperator('+')">+</button>
    </div>

  </div>
</template>

<script>
// 导入 calculator.js 里的方法 Import the method inside calculator.js
import { calculatorMethods } from './assets/calculator.js';
`export default {`
  `data() {`
    `return {`
      `result: '0',`
      `operator: null,`
      `firstValue: null,`
      `secondValue: null`
    `};`
  `},`
  `methods: calculatorMethods`
`};`
</script>


<style scoped>
/* 样式部分已经放入 styles.css 
The style section has been put into styles.css*/
</style>


***Finally, here is the `main.js` file.***

`import { createApp } from 'vue';`

`import App from './App.vue';`

`const app = createApp(App);`

`app.mount('#app');`

***The resulting output is shown in the video below.***

<video src="pictures\10月20日.mp4"></video>

That's the complete tutorial on Vue.js. If you want to dive deeper into learning Vue.js, you can explore related resources on GitHub for further study.