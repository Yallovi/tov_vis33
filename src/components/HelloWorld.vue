<template>
  <div class="container">
    <h1>Чат на основе Firebase</h1>
    <div class="alert alert-primary">adgadsgdsaga</div>
    <div class="block-mess">
      <img src="../assets/feedback-ico__1.jpg" alt="Avatar" />
      <p class="block-mess_text">Hello. How are you today?</p>
      <span class="time-right">11:00</span>
    </div>
    <!-- /.blok-mess -->
    <div class="block-mess two">
      <img src="../assets/feedback-ico__2.jpg" alt="Avatar" class="right" />
      <p class="">Hey! I'm fine. Thanks for asking!</p>
      <span class="time-left">11:01</span>
    </div>
    <!-- /.block-mess_two -->
    <div class="block-mess">
      <img src="../assets/feedback-ico__1.jpg" alt="Avatar" />
      <p class="block-mess_text">Sweet! So, what do you wanna do today?</p>
      <span class="time-right">11:02</span>
    </div>
    <!-- /.block-mess -->
    <div class="block-mess two">
      <img src="../assets/feedback-ico__2.jpg" alt="Avatar" class="right" />
      <p>Nah, I dunno. Play soccer.. or learn more coding?</p>
      <span class="time-left">11:05</span>
    </div>
    <!-- /.block-mess two-->
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* Chat containers */
.block-mess {
  border: 2px solid #dedede;
  background-color: #f1f1f1;
  border-radius: 5px;
  padding: 10px;
  margin: 10px 0;
}

/* Darker chat container */
.two {
  border-color: #ccc;
  background-color: #ddd;
}

/* Clear floats */
.block-mess::after {
  content: "";
  clear: both;
  display: table;
}

/* Style images */
.block-mess img {
  float: left;
  max-width: 60px;
  width: 100%;
  margin-right: 20px;
  border-radius: 50%;
}

/* Style the right image */
.block-mess img.right {
  float: right;
  margin-left: 40px;
  margin-right: 0;
}
.block-mess_text {
  float: left;
}
.block-mess_text .two {
  float: left;
}
/* Style time text */
.time-right {
  float: right;
  color: #aaa;
}

/* Style time text */
.time-left {
  float: left;
  color: #999;
}
</style>
