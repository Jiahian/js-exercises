<template>
   <h1 class="text-3xl">Question 3</h1>
</template>

<script>
    export default {

    }

    const items = [
        {
            title: 'trousers',
            id: 1,
            color: 'blue'
        },
        {
            title: 'shirt',
            id: 2,
            color: 'green'
        },
        {
            title: 'coat',
            id: 3,
            color: 'yellow'
        }
    ]

    const cards = items.map(n=>{ 
        <div class="card-container">
            <div class="card-content">
                <p class="card-title">
                    n.title
                </p>
                <div class="card-footer">
                    <p class="card-text">n.id</p>
                </div>
            </div>
        </div>})

        console.log(cards)
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");
      .card-container {
        font-family: "Roboto", sans-serif;
        filter: drop-shadow(0px 1px 25px rgba(0, 0, 0, 0.25));
        width: 360px;
        border-radius: 12px;
        border: 0.5px solid rgba(0, 0, 0, 0.25);
        margin-right: 24px;
        margin-bottom: 48.5px;
      }

      .card-image {
        width: 100%;
        border-top-left-radius: 12px;
        border-top-right-radius: 12px;
      }

      .card-content {
        padding: 20px 24px;
      }

      .card-text {
        font-size: 16px;
        line-height: 24px;
        color: #21252c;
        margin: 0 0 16px 0;
      }

      .card-footer {
        display: flex;
        flex-direction: row;
      }

      .card-social-logo {
        margin-right: 8px;
      }

      .card-social-text {
        font-weight: 500;
        font-size: 16px;
        line-height: 24px;
        color: #056dff;
        text-decoration: none;
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
</style>