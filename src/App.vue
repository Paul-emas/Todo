<template>

  <div class="app">
    <formBox v-if="show"></formBox>
    <div class="toggle">
      <div class="toggle__lines"></div>
      <div class="toggle__lines"></div>
      <div class="toggle__lines"></div>
    </div>

    <div class="sec-container">
      <div class="fl w-60 sec-header">
        <div class="sec-header--content">
          <h2 class="sec-title">Your <br> Things</h2>
          <p class="sec-date">Mar 18, 2020</p>
        </div>
      </div>

      <div class="fl w-40 sec-analysis">
        <div class="sec-counter--box">
          <div class="sec-counter fl w-50">
            <h2 class="counter">23</h2>
            <p class="sec-counter--caption">Personal</p>
          </div>
          <div class="sec-counter fl w-50">
            <h2 class="counter">15</h2>
            <p class="sec-counter--caption">Business</p>
          </div>

          <div class="sec-percentage--box">
            <h3 class="sec-percentage"><i class="fas fa-spinner fa-spin"></i> 65% done</h3>
          </div>
        </div>
      </div>
    </div>

    <div class="list-container">
      <h1 class="list-caption">Inbox</h1>
      <ul class="list-box">
        <li class="list-items list-meeting">
          <i class="fad fa-briefcase"></i>
          <div class="list-info">
            <p class="list-info--details">Attend a meeting with Fred</p>
            <p class="list-info--caption">Lorem ipsum dolor sit amet consectetur </p>
          </div>
          <p class="list-info--time">7PM</p>
        </li>
        <li class="list-items list-home">
          <i class="fad fa-home"></i>
          <div class="list-info">
            <p class="list-info--details">Wash the dishes</p>
            <p class="list-info--caption">Lorem ipsum dolor sit amet consectetur </p>
          </div>
          <p class="list-info--time">7PM</p>
        </li>
        <li class="list-items list-food">
          <i class="fad fa-utensils-alt"></i>
          <div class="list-info">
            <p class="list-info--details">Buy some tomatoes for rice & stew</p>
            <p class="list-info--caption">Lorem ipsum dolor sit amet consectetur </p>
          </div>
          <p class="list-info--time">7PM</p>
        </li>
        <li class="list-items list-hangout">
          <i class="fad fa-users"></i>
          <div class="list-info">
            <p class="list-info--details">Playing football with small</p>
            <p class="list-info--caption">Lorem ipsum dolor sit amet consectetur </p>
          </div>
          <p class="list-info--time">7PM</p>
        </li>
        <li class="list-items list-meeting">
          <i class="fad fa-briefcase"></i>
          <div class="list-info">
            <p class="list-info--details">Attend a meeting with Fred</p>
            <p class="list-info--caption">Lorem ipsum dolor sit amet consectetur </p>
          </div>
          <p class="list-info--time">7PM</p>
        </li>
        <li class="list-items list-home">
          <i class="fad fa-home"></i>
          <div class="list-info">
            <p class="list-info--details">Wash the dishes</p>
            <p class="list-info--caption">Lorem ipsum dolor sit amet consectetur </p>
          </div>
          <p class="list-info--time">7PM</p>
        </li>
        <li class="list-items list-food">
          <i class="fad fa-utensils-alt"></i>
          <div class="list-info">
            <p class="list-info--details">Buy some tomatoes for rice & stew</p>
            <p class="list-info--caption">Lorem ipsum dolor sit amet consectetur </p>
          </div>
          <p class="list-info--time">7PM</p>
        </li>
        <li class="list-items list-hangout">
          <i class="fad fa-users"></i>
          <div class="list-info">
            <p class="list-info--details">Playing football with small</p>
            <p class="list-info--caption">Lorem ipsum dolor sit amet consectetur </p>
          </div>
          <p class="list-info--time">7PM</p>
        </li>
      </ul>
    </div>

    <div class="nav-box">
      <p class="nav-box--complete">5 completed</p>

      <i class="fal fa-plus nav-box--btn" @click="toggleBox()"></i>
    </div>
  </div>
</template>

<script>
  import Form from './components/Form.vue';

  export default {
    data: function() {
      return {
        show: true
      }
    },

    components: {
      "formBox": Form
    },

    methods: {
      toggleBox() {
        this.show = true;
      }
    }
  }
</script>

<style>

</style>