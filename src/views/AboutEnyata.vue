<template>
<div class="about-wrapper">
    <h2 class="about-header">About Enyata</h2>
    <p class="about-enyata">
      We are a technology company providing engineering-as-a-service solutions at 
    scale to organizations across multiple industries. Our expert teams of engineers, 
    data scientists, designers, and product managers aggregate decades of industry experience. 
    Innovation and sustainability are at the core of the work we do at Enyata, and that is why our clients trust us.
  </p>
  <button @click.prevent="back" class="go-back">Go back</button>
</div>
</template>

<script>
export default {
    methods: {
        back() {
            this.$router.go(-1) // steps to go back to history
        }
    }
}
</script>

<style scoped>
.about-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.about-enyata {
  width: 40%;
  line-height: 20px;
  text-align: center;
  margin-top: 20px;
  margin-right: auto;
  margin-left: auto;
  line-height: 36px;
}
.about-header {
    color: #3F4FD7;
}
.go-back {
    background-color: rgb(221, 221, 221);
    padding: 14px;
    color: rgb(80, 80, 80);
    outline: none;
    border-radius: 6px;
    border: none;
    font-family: 'Poppins';
    width: 8%;
    margin-left: auto;
    margin-right: auto;
}
.go-back:hover {
    background-color: honeydew;
}
</style>