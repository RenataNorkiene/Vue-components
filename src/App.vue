<template>
<div>
  <active-user :name="user.name" :age="user.age"></active-user>
  <user-data @set-data="setUserData"></user-data>
</div>
</template>

<script>
import ActiveUser from "@/components/ActiveUser";
import UserData from "@/components/UserData";
export default {
  name: "App",
  components: {UserData, ActiveUser},
  data() {
    return {
      user: {
        name: 'Renata Norkiene',
        age: 36,
      }
    };
  },
  methods: {
    setUserData(name, age){
      this.user = {
        name: name,
        age: +age,
      };
    }
  }
}
</script>
