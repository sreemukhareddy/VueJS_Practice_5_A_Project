<template>
    <div>
        <h1>Trade or view your portfolio.</h1>
        <h6>You may Save & Load your Data</h6>
        <p> Your funds {{ funds | currency }} </p>
    </div>
</template>

<script>
export default {
  computed: {
    funds(){
        return this.$store.getters.funds;
    }   
  }
}
</script>