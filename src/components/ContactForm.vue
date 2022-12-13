
 <template>
  <div class="contactForm">
    <div class="mb-3">
      <label for="exampleFormControlInput1" class="form-label">Email address</label>
      <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="name@example.com">
    </div>
    <div class="mb-3">
      <label for="exampleFormControlTextarea1" class="form-label">Example textarea</label>
      <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
    </div>
    <div class="d-grid gap-2 d-md-block">
      <button class="btn btn-primary" type="submit" v-on:click="display('Done!')">Submit</button>
    </div>
  </div>
 </template>
 <script>
// submit(){
//                 alert(`${this.fullname} with the email ${this.email} at age ${this.age} was born on ${this.dob}`)
// }
export default {
    name: 'contactForm',
    methods: {
      display: function(item){

        alert(item)
      }
    }
  }
</script>