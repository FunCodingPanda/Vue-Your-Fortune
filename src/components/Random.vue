<template>
  <div class="randomize">
    <h1>{{ msg }}</h1>
    <p>
      Want to play Amigo? Click the button below.
    </p>
    <button @click="random" class="b">Destiny</button>
    <div class="display">{{ current }} </div>
    <div class="message">{{ message }} </div>
  </div>
</template>

<script>
export default {
  name: 'Random',
  props: {
    msg: String
  },
  data() {
    return {
      current: '', 
      message: ''
    }
  },
  methods: {
    random(){
      this.current = Math.floor((Math.random() * 20) +1)
      switch (this.current) {
        case 1: 
          this.message = "Eat something new this week, and you will feel great next week."
          break;
        case 2: 
          this.message = "Mirror, mirror who is the prettiest one of them all? The mirror replied, It's you!"
          break;
        case 3: 
          this.message = "Dooms day is coming!"
          break;
        case 4: 
          this.message = "Do something new this week, and you will meet someone special!"
          break;
        case 5: 
          this.message = "The next you consume something at a Chinese resturant that you think it is chicken, well it is not!"
          break;
        case 6: 
          this.message = "Treat someone to a beer, and you will get one back soon!"
          break;
        case 7: 
          this.message = "You will encounter something dangerous in any shape or form!"
          break;
        case 8: 
          this.message = "This week is your lucky week!"
          break;
        case 9: 
          this.message = "If you dream of something interesting, don't ignore it because it is secretly telling you something that is going to happen in the near future!"
          break;
        case 10: 
          this.message = "You will meet someone special if you travel South East!"
          break;
        case 11: 
          this.message = "Make someones day today, and someone will make your day a year from now!"
          break;
        case 12: 
          this.message = "This upcoming Halloween, do something crazy, you won't regret it"
          break;
        case 13: 
          this.message = "You may want to stay at home for the next week for your own safety!"
          break;
        case 14: 
          this.message = "You will see love down the road in the very near future!"
          break;
        case 15: 
          this.message = "You are on way your way there to success! You are almost there, be patient."
          break;
        case 16: 
          this.message = "In your past life, you were a professional baseball player."
          break;
        case 17: 
          this.message = "You need saving from yourself!"
          break;
        case 18: 
          this.message = "In the next 5 years, you will fall so hard in love that you could not get back up! It is like MMA, but with your heart."
          break;
        case 19: 
          this.message = "You will get a second chance to do something all over again!"
          break;
        case 20: 
          this.message = "It is never over until it is over."
      }
    }
  }
}
</script>

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

.display {
  background-color: white;
  color: black;
  font-size: 50px;
}

.b {
  font-size: 20px;
  padding: 12px 30px;
  border-radius: 12px;
}

</style>
