<script setup>
import PlayIcon from "./icons/PlayIcon.vue";
import SearchIcon from "./icons/SearchIcon.vue";
import RoundIcon from "./icons/RoundIcon.vue";
</script>
<template>
  <section>
    <div class="slider flex flex-center">
      <img
        class="no-select no-drag"
        src="../../public/images/morocco.jpg"
        alt="Slider"
      />
    </div>

    <div class="slide-container flex flex-center flex-y-down">
      <div class="header flex flex-y-center flex-x-between">
        <div class="logo">
          <img src="../../public/favicon.ico" alt="" srcset="" />
        </div>
        <div class="search_box flex flex-center">
          <div class="icon flex flex-center">
            <SearchIcon />
          </div>
          <div class="search">
            <input
              type="search"
              placeholder="Search a peaceful places..."
              name="search"
              id="searching"
            />
          </div>
        </div>
      </div>

      <div class="title">
        <div class="line-box flex flex-y-center flex-x-even">
          <span>Introducing Middle East</span>
          <div class="line"></div>
        </div>
        <h1>Morocco</h1>

        <div class="play flex flex-center">
          <PlayIcon />
          <div class="layer flex flex-center">
            <svg viewBox="0 0 101 101" >
              <path
                fill="none"
                stroke="#ffff"
                d="M7 95C7 46 46 7 95 7"
                stroke-width="5"
                style=""
                transform="matrix(1, 0, 0, 1, 8.881784197001252e-16, 0)"
              />
            </svg>
          </div>
        </div>
      </div>

      <div class="bottom flex flex-y-center">
        <div class="nav flex flex-center active">
          <RoundIcon />
        </div>
        <div class="nav flex flex-center">
          <RoundIcon />
        </div>
        <div class="nav flex flex-center">
          <RoundIcon />
        </div>
        <div class="nav flex flex-center">
          <RoundIcon />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.layer {
  top: 0;
  left: 0;
  width: 30px;
  height: 30px;
  position: absolute;
}

.nav {
  width: 15px;
  height: 15px;
  opacity: 0.7;
  margin-left: 10px;
}
.nav.active {
  width: 20px;
  height: 20px;
  opacity: 1;
  border-radius: 50%;
  border: solid 1px #fff;
}
.bottom {
  bottom: 0;
  width: 100%;
  padding: 40px 0;
  position: absolute;
  margin-left: 90px;
}
.logo {
  width: 60px;
  height: 60px;
  margin-left: 30px;
}
.header {
  top: 0;
  left: 0;
  width: 100%;
  padding: 30px 0;
  position: absolute;
}
.header input,
.header input::placeholder {
  width: 100%;
  color: #fff;
  font-weight: 100;
}
.header .search {
  width: 300px;
}
.icon {
  width: 20px;
  height: 20px;
  margin-right: 10px;
}
.play {
  position: relative;
  width: 65px;
  height: 65px;
  padding: 25px;
  margin-top: 30px;
  margin-left: 380px;
  background: #ffffff3d;
  backdrop-filter: blur(15px);
  border-radius: 50%;
  transform: rotate(80deg);
}

.play-ic {
  transform: rotate(-80deg);
}

.line-box {
  position: absolute;
  margin-left: 280px;
}
.line {
  width: 50px;
  height: 1px;
  margin-left: 20px;
  background: #fff;
}
.slider {
  width: 100%;
  height: 100vh;
  overflow: hidden;
  position: relative;
}

.slider::after {
  top: 0;
  left: 0;
  content: "";
  width: 100%;
  height: 100%;
  opacity: 0.2;
  position: absolute;
  background: black;
}

.slider img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.slide-container {
  top: 0;
  width: 50%;
  height: 100vh;
  position: absolute;
}
.title {
  color: #fff;
}
.title h1 {
  font-size: 7rem;
  font-weight: 600;
  color: #fff;
}
</style>
