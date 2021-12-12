<template>
<MyBtn :color="color" text="Banana" />
<MyBtn color="royalblue" text="Apple" />
<MyBtn large text="Cherry" />
<MyBtn text="Melon" /><br>
<Btn @click="log" @change-msg="logMsg">Seyoung</Btn>

<Parent :message="message" />
</template>

<script>
import MyBtn from './components/MyBtn'
import Btn from './components/Btn'

export default {
  components: {
    MyBtn,
    Btn
  },

  methods: {
    log() {
      console.log('click')
    },

    logMsg(msg) {
      console.log(msg)
    },

  data() {
    return{
      color: '#000',
      }
    },

  }
}
</script>
