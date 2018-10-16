<template>
  <div class="home">
    <div>
        <ul>
          <li v-for="person in people" v-on:click="listOfPeople(person)">{{ person.name }}</li>
        </ul>
      </div>
  </div>
</template>

<style>
</style>

<script>
export default {
  data: function() {
    return {
      people: [
      {name: "Homer", bio: "works at powerplant", bioVisible: true},
      {name: "Mr.Burns", bio: "filthy rich", bioVisible: true}
      ]
    };
  },
  created: function() {},
  methods: {},
  computed: {}
};
</script>