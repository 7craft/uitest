<!--this is a card of user info-->
<template>
  <div class="card card-user">
    <div class="image">
      <img src="" alt="">
    </div>
    <div class="content">
      <div class="author">
        <img class="avatar border-white" src="" alt="">
        <h4 class="title">Project Manager
          <br>
          <a href="#">
            <small>@SmartFishPond</small>
          </a>
        </h4>
      </div>
      <p class="description text-center">
        
        <br> 
        <br> 
      </p>
    </div>
    <hr>
    <div class="text-center">
      <div class="row">
        <div v-for="(info,index) in details" :class="getClasses(index)">
          <h5>{{info.title}}
            <br>
            <small>{{info.subTitle}}</small>
          </h5>
        </div>
      </div>
    </div>
  </div>
</template>



<script>
  export default {
    data () {
      return {
        details: [
          {
            title: '123',
            subTitle: 'Test'
          },
          {
            title: '123',
            subTitle: 'Test'
          },
          {
            title: '123',
            subTitle: 'Test'
          }
        ]
      }
    },
    methods: {
      getClasses (index) {
        var remainder = index % 3
        if (remainder === 0) {
          return 'col-md-3 col-md-offset-1'
        } else if (remainder === 2) {
          return 'col-md-4'
        } else {
          return 'col-md-3'
        }
      }
    }
  }

</script>
<style>
  
</style>
