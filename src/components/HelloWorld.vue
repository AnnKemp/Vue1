<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      For a guide and recipes on how to configure / customize this project,<br />
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener"
        >vue-cli documentation</a
      >.
    </p>
    <h3>Installed CLI Plugins</h3>
    <ul>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel"
          target="_blank"
          rel="noopener"
          >babel</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-router"
          target="_blank"
          rel="noopener"
          >router</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint"
          target="_blank"
          rel="noopener"
          >eslint</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-typescript"
          target="_blank"
          rel="noopener"
          >typescript</a
        >
      </li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li>
        <a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a>
      </li>
      <li>
        <a href="https://forum.vuejs.org" target="_blank" rel="noopener"
          >Forum</a
        >
      </li>
      <li>
        <a href="https://chat.vuejs.org" target="_blank" rel="noopener"
          >Community Chat</a
        >
      </li>
      <li>
        <a href="https://twitter.com/vuejs" target="_blank" rel="noopener"
          >Twitter</a
        >
      </li>
      <li>
        <a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a>
      </li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li>
        <a href="https://router.vuejs.org" target="_blank" rel="noopener"
          >vue-router</a
        >
      </li>
      <li>
        <a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a>
      </li>
      <li>
        <a
          href="https://github.com/vuejs/vue-devtools#vue-devtools"
          target="_blank"
          rel="noopener"
          >vue-devtools</a
        >
      </li>
      <li>
        <a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener"
          >vue-loader</a
        >
      </li>
      <li>
        <a
          href="https://github.com/vuejs/awesome-vue"
          target="_blank"
          rel="noopener"
          >awesome-vue</a
        >
      </li>
    </ul>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "HelloWorld",
  props: {
    msg: String
    // for tutorial check Adam's real world vue 3 typescript course.
    // code see: github.com/code-pop/Real-World-Vue-3-TypeScript
 }
});
// some new types
//tuple type = fixed array with predefined data types
//Enum type = allows you to define friendly names to a set of values vb: enum ArrowKeys{
//  Up, Down, Left, Right}

// let shoppingList:string[]=['apple', 'bananas', 'peers']; // how to define type for an array, the string is the type that's in the array
// How to apply type to an object // let person: { name:string; age: number;}={name:'Peter Parker, age:20}
// beter is het echter om met een interface te werken, vb: interface Hero={ name: string; age: number; activeAdvenger: boolean; powers: string[];} let person: Hero={name: 'Peter Parker', age: 20, activeAdvenger: true, powers: ['wall-crawl', 'spider-sense']}
// adding type to a function: let generateFullName=(firstName: string, lastName: string): string=> {
 // return firstName + ' ' + lastName} //  de typering achter het dubbelpunt na de gebogen haakjes dient om het type van het resultaat van de functie te bepalen
 // Defining custom types: type buttonType='primary' | 'secondary' | 'succes' | 'danger' // de rechte streep is een Union Operator en betekent 'of' in Typescript   let buttonStyles: buttonType='primary' // dus hier maak je zelf je op maak gemaakte typeringen

// for advanced typescript in Vue install extension: 'vuedx' in Visual Studio Code
// const futureTodoItem = {} as TodoItem // with the 'as' we override typescript and can add content to an empty constante
// futureTodoItem.label='Install VueDX extension'
// futureTodoItem.completed= true
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
