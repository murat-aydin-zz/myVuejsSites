<template>
  <z-view label="Murat AYDIN" label-pos="bottom">
    <img class="mainclass" src="https://scontent-frt3-1.xx.fbcdn.net/v/t31.0-8/18623536_10209065620069341_871261362345751032_o.jpg?_nc_cat=0&oh=4c832da2333f05d8a3e0541cfd2cb30c&oe=5C249BC1"
    >
    <div slot="extension">
      <!-- status monitor -->
        <z-spot
                style="background-color: orange; border-width: 4px; border-color: var(--background-color);"
                :angle="-145"
                size="m"
                :distance="120"
                to-view="status">
          <i style="color: var( --accent-text-color)" class="fas fa-bell"></i><br>
          <span style="color: var( --accent-text-color)">15</span>
        </z-spot>
      <!-- family-->
      <z-spot
<<<<<<< HEAD
              :angle="-30"
              size="s"
              :distance="120"
              label="Harita"
              label-pos="top"
              to-view="family">
        <i class="fas fa-map-marker-alt"></i>
=======
        :angle='45'
        to-view='docs'
        class='accent'
        label='Docs'>
        <i class='fas fa-book'></i>
>>>>>>> cb9d8ea10ad0f65f40baaccbf81009f26267fbbf
      </z-spot>
      <z-spot slot="extension"
              button
              :angle="90"
              size="xxs"
              :style=" 'on' ? 'border-color: green; background-color: green;' : 'border-color: red; background-color: red;'">
      </z-spot>
      <!-- scenes-->
      <z-spot
              :angle="0"
              size="s"
              :distance="120"
              label="İletişim"
              label-pos="right"
              to-view="scenes">
        <i class="fab fa-phoenix-framework"></i>
      </z-spot>
      <!-- rooms-->
      <z-spot
              :angle="30"
              size="s"
              :distance="120"
              label="Deneyim"
              label-pos="right"
              to-view="rooms">
        <i class="fas fa-briefcase"></i>
      </z-spot>
      <!-- devices-->
      <z-spot
              :angle="60"
              :distance="120"
              size="s"
              label="Yetenekler"
              label-pos="right"
              to-view="devices">
        <i class="fas fa-chart-line"></i>
      </z-spot>
      <!-- settings-->
      <z-spot
<<<<<<< HEAD
              :angle="150"
              :distance="120"
              size="s"
              label="Ayarlar"
              to-view="setting">
        <i class="fas fa-sliders-h"></i>
=======
        button
        :angle='135'
        class='accent'
        label='Github'
        @click.native="openUrl">
        <i class='fab fa-github'></i>
>>>>>>> cb9d8ea10ad0f65f40baaccbf81009f26267fbbf
      </z-spot>
    </div>
  </z-view>
</template>