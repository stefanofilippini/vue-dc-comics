<template>
    <footer>
        <div class="text-container">
            ciao
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
    
    data() {
      return {
        DcComicsList: [
          {
            url: '/',
            text: 'characters'
          },
          {
            url: '/',
            text: 'comics'
          },
          {
            url: '/',
            text: 'movies'
          },
          {
            url: '/',
            text: 'tv'
          },
          {
            url: '/',
            text: 'games'
          },
          {
            url: '/',
            text: 'videos'
          },
          {
            url: '/',
            text: 'news'
          }
        ],
        shopList: [
          {
            url: '/',
            text: 'shop dc'
          },
          {
            url: '/',
            text: 'shop dc collectibles'
          }
        ],
        dcList: [
          {
            url: '/',
            text: 'term of use'
          },
          {
            url: '/',
            text: 'Privacy policy (new)'
          },
          {
            url: '/',
            text: 'ad choises'
          },
          {
            url: '/',
            text: 'advertising'
          },
          {
            url: '/',
            text: 'jobs'
          },
          {
            url: '/',
            text: 'subscriptions'
          },
          {
            url: '/',
            text: 'talent workshops'
          },
          {
            url: '/',
            text: 'cpsc certificates'
          },
          {
            url: '/',
            text: 'ratings'
          },
          {
            url: '/',
            text: 'shop help'
          },
          {
            url: '/',
            text: 'contact us'
          },
        ],
        sitesList: [
          {
            url: '/',
            text: 'dc'
          },
          {
            url: '/',
            text: 'Mad megazine'
          },
          {
            url: '/',
            text: 'dc kids'
          },
          {
            url: '/',
            text: 'dc universe'
          },
          {
            url: '/',
            text: 'dc power visa'
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>

    footer {
        width: 100%;
        height: 120px;
        background-color: aqua;
        border: 1px solid black;
        .text-container {
            background-color: blue;
        }
    }
</style>