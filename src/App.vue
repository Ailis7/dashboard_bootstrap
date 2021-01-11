<template>
  <div id="dashboard">
    <!-- <first-garantee></first-garantee> -->
    <second-garantee></second-garantee>
  </div>
</template>

<script>
// import { BCard } from "bootstrap-vue";
import FirstGarantee from "./components/FirstGarantee";
import SecondGarantee from "./components/SecondGarantee";
import FirstFactoring from "./components/FirstFactoring";
import SecondFactoring from "./components/SecondFactoring";

export default {
  name: "dashboard",
  components: {
    FirstGarantee,
    SecondGarantee,
    FirstFactoring,
    SecondFactoring
  },
  data() {
    return {};
  },
  methods: {},
  computed: {}
};
</script>

<style>
html {
  font-size: 40px;
  font-family: Roboto-Bold;
}

.col,
.row,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6,
small {
  font-weight: bold;
}

@media screen and (max-width: 1281px) {
  html {
    font-size: 20px;
  }
}

.prev-button,
.next-button {
  display: block;
  width: 2em;
  height: 2em;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  opacity: 0.5;
  background-size: 2em 2em;
}

.prev-button:hover,
.next-button:hover {
  opacity: 1;
  cursor: pointer;
}

.prev-button {
  background-image: url("./svg/arrow-left.svg");
}
.next-button {
  background-image: url("./svg/arrow-right.svg");
}

.bigDigits {
  font-size: 3em;
  line-height: 1;
}
.progress-bar {
  border-radius: 20px;
  background-color: #503aeb;
}

small {
  font-size: 0.65rem;
}

.text-uppercase {
}

.decrease {
  color: #ff7f00;
}

.increase, .increase2{
  color: #67c23a;
}
.increase::before {
    content: "\25b2";/*"\2BC5";*/
    font-size: 50px;
}

.decrease,
.increase, .increase2 {
  font-weight: 500;
  margin-bottom: 0;
  
}
</style>
