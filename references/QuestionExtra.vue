<template>
  <div>
    <h1 class="text-3xl">Question Extra</h1>
    <!-- Qn: Use v-for directive to render a list of items based on a given array. -->
    <!-- Display them in cards form. (Refer to the image in the assets folder) -->
    <!-- There are missing css styling too. -->
    <div class="cards-section">
      <div v-for="item in items"
      :key="item"
      class="card-container">
        <div class="card-image" v-bind:style="{'background-color': item.color}">
            {{item.id}}
        </div>
        <div class="card-content">
          <p class="card-title">
            {{ item.title }}
          </p>
          <p class="card-desc">{{ item.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    data:() => ({
      items: [
        {
            title: 'Trousers',
            id: 1,
            description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
            color: '#75C2EC'
        },
        {
            title: 'Shirt',
            id: 2,
            description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
            color: '#F6C42E'
        },
        {
            title: 'Coat',
            id: 3,
            description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
            color: '#007C00'
        },
        {
            title: 'Dress',
            id: 4,
            description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
            color: '#75C2EC'
        },
        {
            title: 'Blouse',
            id: 5,
            description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
            color: '#F6C42E'
        },{
            title: 'Sock',
            id: 6,
            description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
            color: '#007C00'
        }

      ]
    })
  }

</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");
      .card-container {
        font-family: "Roboto", sans-serif;
        filter: drop-shadow(0px 1px 25px rgba(0, 0, 0, 0.25));
        width: 300px;
        border-radius: 12px;
        border: 0.5px solid rgba(0, 0, 0, 0.25);
        margin-right: 24px;
        margin-bottom: 48.5px;
      }

      .card-image {
        height: 200px;
        width: 100%;
        border-top-left-radius: 12px;
        border-top-right-radius: 12px;
        display: flex;
        justify-content: center;
        align-items: center;
        color: #fff;
        font-size: 5rem;
      }

      .card-content {
        padding: 20px 24px;
      }

      .cards-section {
        display: flex;
        flex-direction: row;
        justify-content: center;
        flex-wrap: wrap;
        max-width: 1440px;
        padding: 0 156px;
        margin: auto;
      }

      .card-title {
        font-weight: bold;
        font-size: 18px;
        margin-bottom: 8px;
      }
</style>