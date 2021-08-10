<template>
  <div class="header-block">
    <h1 class="header-block__title"> Minesweeper </h1>
      <div>
        <img class="header-block__image" src="@/assets/bomb.png"/>
      </div>
      <!-- <a href="#" class="start">О игре</a> -->
      <!-- <div class="header-block__text" 
        data-text="Целью игры является открытие всех ячеек, не содержащих мины. 
        Игрок открывает ячейки, стараясь не открыть ячейку с миной. Открыв ячейку с миной, он проигрывает. 
        Мины расставляются после первого хода, поэтому в новых версиях проиграть на первом же ходу невозможно.">
      </div> -->
      <div class="header-block__text">
        Целью игры является открытие всех ячеек, не содержащих мины. 
        Игрок открывает ячейки, стараясь не открыть ячейку с миной. Открыв ячейку с миной, он проигрывает. 
        Мины расставляются после первого хода, поэтому в новых версиях проиграть на первом же ходу невозможно.
      </div>
      <div class="block-info__btn">
      <router-link to="/game" class="block-info__button block-info__start">START</router-link>
      </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  components: {
  },
  // data: function typeWriter(text, n) {
  // if (n < (text.length)) {
  //   ('.header-block__image').html(text.substring(0, n+1));
  //   n++;
  //   setTimeout(function() {
  //     typeWriter(text, n)
  //   }, 100);
  // }
    // ('.start').click(function(e) {
    //   e.stopPropagation();
    //   var text = ('.header-block__image').data('text');
    //   typeWriter(text, 0);
    // })
  // }
}
</script>

<style lang="scss" scoped>
@import "~@openfonts/kumar-one-outline_all/index.css";
.header-block {
  &__title {
    color: #f54768;
    font-family: "Kumar One Outline", cursive;
    font-weight: normal;
    text-align: center;
  }
  &__text {
    padding: 10px;
  }
  &__image {
    display: block;
    margin-right: auto;
    margin-left: auto;
    width: 200px;
  }
}
  .block-info{
    &__btn {
      display: flex;
      justify-content: space-around;
      padding: 20px;
    }
    &__button {
      background-color: #111;
      border: solid 1px #888;
      color: #888;
      padding: 8px 25px;
      font-size: 26px;
      letter-spacing: 2px;
      cursor: pointer;
    }
    &__start {
      // position: absolute;
      // top: 50%;
      // left: 50%;
      // transform: translate(-50%, -50%);
    }
  }
</style>
