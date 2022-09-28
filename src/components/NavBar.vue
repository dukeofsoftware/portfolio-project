<template lang="">
<!--   <nav class="navbar navbar-dark bg-success navbar-expand-sm bg-navbar">
    <div class="container">
      <div class="collapse navbar-collapse">
        <ul class="navbar-nav">
          <li class="navbar-item">
            <router-link
              @click="hangisinde"
              to="/"
              class="nav-link px-3"
              :class="brandcolor()"
              >Ana Sayfa</router-link
            >
          </li>
          <li class="navbar-item">
            <router-link
              :class="brandcolor2()"
              @click="hangisinde"
              to="/projects"
              class="nav-link px-3"
              >Projeler</router-link
            >
          </li>
          <li class="navbar-item">
            <router-link
              :class="brandcolor3()"
              @click="hangisinde"
              to="/contact"
              class="nav-link px-3"
              >İletişim</router-link
            >
          </li>
        </ul>
      </div>
    </div>
  </nav> -->
  <div class="navbar bg-base-100 border-black">
    <div class="flex-1">
        <router-link
          @click="hangisinde"
          to="/"
          class="nav-link px-3"
          :class="brandcolor()"
          >Ana Sayfa</router-link>
        
    </div>
    <div class="flex-none">
      <ul class="menu menu-horizontal p-0">
        <li class="navbar-item">
          <router-link
            :class="brandcolor2()"
            @click="hangisinde"
            to="/projects"
            class="nav-link px-3"
            >Projeler</router-link
          >
        </li>
      
        <li class="navbar-item">
          <router-link
            :class="brandcolor3()"
            @click="hangisinde"
            to="/contact"
            class="nav-link px-3"
            >İletişim</router-link
          >
        </li>
      </ul>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      isMain: true,
      isContact: false,
      isProject: false,
    };
  },
  methods: {
    hangisinde: function (event) {
      if (event.target.innerHTML === "Ana Sayfa") {
        this.isMain = true;
        this.isContact = false;
        this.isProject = false;
      } else if (event.target.innerHTML === "İletişim") {
        this.isMain = false;
        this.isContact = true;
        this.isProject = false;
      } else if (event.target.innerHTML === "Projeler") {
        this.isMain = false;
        this.isContact = false;
        this.isProject = true;
      }
    },
    brandcolor: function () {
      return {
        "navbar-brand": this.isMain && !this.isContact && !this.isProject,
      };
    },
    brandcolor2: function () {
      return {
        "navbar-brand":this.isProject,
      };
    },
    brandcolor3: function () {
      return {
        "navbar-brand": this.isContact
      };
    },
  },
};
</script>
<style>
.bg-navbar {
  background: rgb(2, 0, 36);
  background: linear-gradient(
    90deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(68, 9, 121, 1) 36%,
    rgba(85, 0, 255, 0.9907407407407407) 100%
  );
}
</style>
