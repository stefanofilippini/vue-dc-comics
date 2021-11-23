<template>
  <header>
      <div class="text-container">
          <a href="#">
              <img src="../assets/dc-logo.png" alt="Logo">
          </a>

          <ul>
              <li v-for="(link, index) in DcComicsList" :key="`key-${index}`">
                  <a href="#">{{ link.text }}</a>
              </li>
          </ul>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header',
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
            text: 'fans'
          },
          {
            url: '/',
            text: 'news'
          },
          {
            url: '/',
            text: 'shop'
          },
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

    header {
        display: flex;
        width: 100%;
        height: 120px;
        .text-container {
            display: flex;
            align-items: center;
            a {
                display: flex;
                align-items: center;
                height: 100%;
                img {
                    height: 64%;
                    margin-left: 25px;
                }
            }
            ul {
                flex-grow: 1;
                display: flex;
                height: 100%;
                justify-content: flex-end;
                align-items: center;
                li {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    justify-self: flex-end;
                    list-style: none;
                    height: 100%;
                    margin-left: 25px;
                    text-transform: uppercase;
                    font-weight: 700;
                    font-size: 12px;
                    border-bottom: 5px solid transparent;
                    color: black;
                    &:hover {
                        color: #1a75f2;
                        border-bottom: 5px solid #1a75f2;
                        a {
                            color: #1a75f2;
                        }
                    }
                    a {
                        color: black;
                        text-decoration: none;
                    }
                }
            }
        }
}
</style>