<template>
  <div class="main">
    <section class="container">
      <h2>Обо мне</h2>
      <div class="aboutMePhoto">
        <div class="text">
          Здравствуйте, меня зовут Дарина и я frontend-разработчик.
          Сейчас мне 21 год и уже 5 лет занимаюсь программированием. <br>
          Как и многие, впервые я познакомилась с разработкой в школе,
          после поступила в колледж на специальность "Программирование в компьютерных системах".
          Отучилась 4 года, защитила диплом и решила продолжить развиваться в данной сфере. <br>
          Один из самых сложных этапов был поиск первой работы,
          но немного везения и знакомства помогли мне начать свои первые коммерческие проекты.
          Сейчас я активно самостоятельно развиваюсь и нахожу много нового в любимой профессии.<br>
          Но так как жить только работой утомительно, необходимы хобби и в повседневной жизни.
          Почти все детство я занималась лыжным спортом, потом как почти все подростки забросила,
          ведь так много всего интересного помимо спорта.
          Год назад я вспомнила молодость и вновь начала кататься,
          стало гораздо приятнее заниматься, ведь это мое осознанное решение. <br>
          В свободное время я люблю смотреть сериалы, аниме, играть в игры.
          Имею целую подборку того, что можно посоветовать посмотреть.
          Ниже фотографии меня в старших классах и сейчас, очень верю,
          что за это время достаточно изменилась.
        </div>
        <div class="photos">
          <Photo text="Я в 2023 году" alt="Я сейчас" img="/NewPhoto.jpeg" />
          <Photo text="Много лет назад" alt="Я в старших классах" img="/OldPhoto.jpeg" />
        </div>
      </div>
    </section>
  </div>
</template>

<script lang="ts">
import Photo from "../components/Photo.vue";
export default {
  components: {Photo}
}
</script>

<style>
body {
  background: whitesmoke;
  color: #1B1B1B;
}
.main {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
  padding: 20px;
}
.container {
  font-family: Gill Sans;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
}
.container > div {
  width: 80%;
}
.aboutMePhoto {
  display: flex;
  flex-direction: column;
  gap: 20px;
}
.text {
  text-align: justify;
  font-size: 18px;
  line-height: 25px;
}
.photos {
  display: flex;
  justify-content: center;
  gap: 20px;
}

@media (min-width: 320px) and (max-width: 768px) {
  .container > div {
    width: 100%;
  }
  .main {
    padding: 10px;
  }
  .text {
    font-size: 16px;
  }
}

</style>
