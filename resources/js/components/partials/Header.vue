<template>
  <header>
    <nav class="container"> 
      <ul>
        <li>
          <router-link :to="{name: 'home'}">Home</router-link>
        </li>
        <li>
          <router-link :to="{name: 'blog'}">Blog</router-link>
        </li>
        <li>
          <router-link :to="{name: 'about'}">Chi siamo</router-link>
        </li>
        <li>
          <router-link :to="{name: 'contacts'}">Contatti</router-link>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss" scoped>
  header{
    background-color: slategray;
    height: 70px;
    line-height: 70px;
    text-align: center;
    ul{
      list-style: none;
      li{
        display: inline-block;
        margin: 0 20px;
        a{
          text-decoration: none;
          color: white;
          &:hover{
            text-decoration: underline;
          }
          &.active{
            color: brown;
          }
        }
      }
    }
  }
</style>