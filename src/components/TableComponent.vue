<template>
  <div class="container">
    <h3>{{ title }}</h3>
    <table class="table table-hover" :style="stylecomp" >
      <thead>
        <tr >
          <th  scope="col" v-for="(value, key) in users[0]" :key="key">
            {{ key }}
          </th>
        </tr>
      </thead>
      <tbody >
        <tr  v-for="user in users" :key="user.id">
          <td  v-for="(value, key) in user" :key="key">{{ value }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    users: Array,
    stylecomp: Object,
  },
  data(){
    return {
        
    }
  }

};
</script>

<style>
</style>