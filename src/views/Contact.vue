<template>
  <div class="form-wrapper">
      <form>
        <h3>Contact Us</h3>
        <input class="first-name" type="name" placeholder="First Name" v-model="formData.firstname" />
        <input class="first-name" type="name" placeholder="Last Name" v-model="formData.lastname" />
        <input class="first-name" type="email" placeholder="Email" v-model="formData.email" />
        <input class="first-name" type="tel" placeholder="Phone No." v-model="formData.tel" />
        <textarea class="text-area" rows = "5" cols = "50" name = "description" placeholder="Reason for contacting us" v-model="formData.reason"></textarea>
        <button class="submit-btn" :disabled="!formData.firstname" @click.prevent="submit">Submit</button>
      </form>
  </div>
</template>

<script>
export default {
    data () {
        return {
            formData: {
                firstname: '',
                lastname: '',
                email: '',
                tel: '',
                reason: '',
            }
        }
    },
    methods: {
        submit() {
          alert('Submited')
        }
    }
}
</script>

<style scoped>
.form-wrapper {
    margin-bottom: 20px;
    background: url(../assets/overall-triangle.svg);
    background-repeat: no-repeat;
}
form {
    display: flex;
    flex-direction: column;
    justify-content: center;
}
.first-name {
    padding: 20px;
    width: 36%;
    background: rgb(245, 250, 252);
    box-shadow: rgba(0, 0, 0, 0.02) 0px 1px 3px 0px, rgba(27, 31, 35, 0.15) 0px 0px 0px 1px;
    border: none;
    outline: none;
    border-radius: 6px;
    font-size: 14px;
    margin-right: auto;
    margin-left: auto;
    margin-bottom: 20px;
    font-family: 'Poppins';
}
.text-area {
    width: 36%;
    padding: 20px;
    margin-right: auto;
    margin-left: auto;
    border: none;
    outline: none;
    border-radius: 6px;
    font-size: 14px;
    box-shadow: rgba(0, 0, 0, 0.02) 0px 1px 3px 0px, rgba(27, 31, 35, 0.15) 0px 0px 0px 1px;
    background: rgb(245, 250, 252);
    font-family: 'Poppins';
}
.first-name:focus {
    border: 1px solid #3F4FD7;
}
.submit-btn {
    padding: 14px;
    width: 38%;
    background-color: #3F4FD7;
    color: #fff;
    font-family: 'Poppins';
    margin-left: auto;
    margin-right: auto;
    margin-top: 20px;
    border: none;
    outline: none;
    border-radius: 6px;
    cursor: pointer;
    box-shadow: rgba(0, 0, 0, 0.2) 0px 60px 40px -7px;
    /* box-shadow: rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.04) 0px 10px 10px -5px; */
}
.submit-btn:disabled {
    background: rgb(224, 224, 223);
    color: #000;
}
.submit-btn:disabled:hover {
    background: rgb(224, 224, 223);
    color: #000;
}
.submit-btn:hover {
    background-color: #131f8f;
}
</style>