<script setup>
import BackIcon from "./icons/BackIcon.vue";
import FireIcon from "./icons/FireIcon.vue";
import CommentIcon from "./icons/CommentIcon.vue";
import NavIcon from "./icons/NaveIcon.vue";
</script>
<template>
  <section>
    <div class="header flex flex-center flex-x-between">
      <div class="icon flex flex-center">
        <BackIcon />
      </div>
      <div class="flex flex-y-center">
        <div class="L-Icon flex flex-center active">
          <FireIcon />
        </div>
        <div class="L-Icon flex flex-center">
          <CommentIcon />
        </div>
      </div>
      <div class="icon flex flex-center">
        <NavIcon />
      </div>
    </div>

    <div class="image">
      <img src="../../public/images/mosque.png" alt="Mosque" srcset="" />
    </div>

    <div class="info">
      <div class="info-desc">
        <h2>Welcome to <b>Morocco</b></h2>
        <span
          >Morocco is a land of contrasts, from the snow-capped Atlas Mountains
          to the sandy dunes of the Sahara Desert. It is a country rich in
          history and culture, with ancient medinas, stunning mosques, and
          world-class cuisine. Morocco is also a friendly and welcoming country,
          with warm and hospitable people.</span
        >
      </div>
    </div>

    <div class="navigator flex flex-center T-gray">
      <div class="list">Experiences</div>
      <div class="list active">Photo</div>
      <div class="list">Activities</div>
      <div class="list">Map</div>
    </div>

    <div class="collections flex">
      <div class="cover flex flex-center">
        <img src="../../public/images/M1.jpg" alt="Beautiful Places" />
      </div>
      <div class="cover flex flex-center MT-15px">
        <img src="../../public/images/M6.jpg" alt="Beautiful Places" />
      </div>
    </div>
  </section>
</template>
<style scoped>
.collections {
  width: 100%;
  margin: 0 auto;
  margin-left: 25px;
}
.cover {
  width: 250px;
  height: 300px;
  margin: 20px;
  flex-wrap: wrap;
  overflow: hidden;
  border-radius: 25px;
}
.cover img {
  top: -49px;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.L-Icon {
  width: 50px;
  height: 50px;
  background: #f0f4f7;
  border-radius: 50%;
  padding: 15px;
  margin: 0 10px;
}
.L-Icon.active {
  padding: 15px;
  background: #ffd586;
}
.icon {
  width: 30px;
  height: 30px;
}
.info {
  text-align: center;
}

.info h2 {
  margin-bottom: 30px;
}
.navigator {
  margin: 30px;
  font-weight: 500;
}
.list.active {
  color: black;
  font-size: 1.2rem;
  font-weight: 700;
  position: relative;
}
.list.active::before {
  content: "";
  left: 45%;
  bottom: -5px;
  width: 8px;
  height: 8px;
  background: red;
  border-radius: 50%;
  position: absolute;
}
</style>
