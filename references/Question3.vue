<template>
  <div>
    <h1 class="text-3xl">Question 3</h1>
    <div v-html="displayHtml(people)"/>
  </div>
</template>

<script>
export default {
    data:() => ({
      people: [
      {
        id: 1,
        first_name: "Dory",
        last_name: "Cutress",
        email: "dcutress0@photobucket.com",
        job: "Account Executive",
      },
      {
        id: 2,
        first_name: "Prisca",
        last_name: "Hatto",
        email: "phatto1@go.com",
        job: "VP Quality Control",
      },
      {
        id: 3,
        first_name: "Tilly",
        last_name: "Noddles",
        email: "tnoddles2@webeden.co.uk",
        job: "Account Executive",
      },
    ]
  }),
  props: {
    html : {
      type: String, 
      default:""
    }
  },
  methods: {
    displayHtml(people) {

      // Qn: Display a list of people's full name using the array map funciton
      // Expected output:
      // - Dory Cutress
      // - Prisca Hatto
      // - Tilly Noddles

      // Concepts: 
      // - object, array
      // - mapping
      // - function

      //Ans: 
      function createList(person){
        return '<li>' + person.first_name + " " + person.last_name + '</li>'
      }
      const list = people.map(createList)
      const html = '<ul>' + list.join('') + '</ul>';
      return html;
    }
  }

}
</script>

<style>
ul {
  list-style-type: initial;
  margin: 16px;
  padding: 16px;
}
</style>