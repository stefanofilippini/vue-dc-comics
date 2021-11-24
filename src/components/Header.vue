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
        ],
        cards: [
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX',
        price: '$19.99',
        series: 'Action Comics',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01',
        price: '$3.99',
        series: 'American Vampire 1976',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb',
        price: '$16.99',
        series: 'Aquaman',
        type: 'graphic novel',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76',
        price: '$2.99',
        series: 'Batgirl',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
        price: '$3.99',
        series: 'Batman',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
        price: '$2.99',
        series: 'Batman Beyond',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8',
        price: '$3.99',
        series: 'Batman/Superman',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk',
        price: '$4.99',
        series: 'Batman/Superman Annual',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8',
        price: '$5.99',
        series: 'Batman: The Joker War Zone',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY',
        price: '$6.99',
        series: 'Batman: Three Jokers',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX',
        price: '$4.99',
        series: 'Batman: White Knight Presents: Harley Quinn',
        type: 'comic book',
    },
    {
        thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq',
        price: '$16.99',
        series: 'Catwoman',
        type: 'graphic novel',
    },
        ],
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