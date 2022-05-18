<template>
  <header class="header">
    <div class="container">
      <div class="header__logo">
        <img src="../assets/dc-logo.png" alt="" />
      </div>
      <nav>
        <ul class="header__menu">
          <li
            v-for="(item, index) in headerLinks"
            :key="index"
            :class="{ active: item.active }"
          >
            <a href="">{{ item.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "MyHeader",
  data() {
    return {
      headerLinks: [
        {
          ulr: "#",
          text: "Characters",
          active: false,
        },
        {
          ulr: "#",
          text: "Comics",
          active: true,
        },
        {
          ulr: "#",
          text: "Movies",
          active: false,
        },
        {
          ulr: "#",
          text: "TV",
          active: false,
        },
        {
          ulr: "#",
          text: "Games",
          active: false,
        },
        {
          ulr: "#",
          text: "Collectibles",
          active: false,
        },
        {
          ulr: "#",
          text: "Videos",
          active: false,
        },
        {
          ulr: "#",
          text: "Fans",
          active: false,
        },
        {
          ulr: "#",
          text: "News",
          active: false,
        },
        {
          ulr: "#",
          text: "Shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/variables.scss";

.container {
  height: 150px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header {
  nav {
    width: 80%;
  }
  &__menu {
    list-style: none;
    display: flex;
    justify-content: space-between;

    li {
      text-transform: uppercase;
      font-weight: bold;
      line-height: 147px;
      a {
        color: $header-text-color;
      }
    }

    li.active {
      border-bottom: 3px solid $brand-primary-color;
    }

    li.active a {
      color: $brand-primary-color;
    }
  }

  &__logo {
    width: 100px;
  }
}
</style>
