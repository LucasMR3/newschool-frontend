<template>
  <div class="full__height">
      <v-container fluid class="wrapper__without__content full__height">
        <v-row class="full__height">
          <v-col cols="12">
            <h1 class="full__width text__without__content">{{title}}</h1>
            <p class="full__width">{{message}}</p>
          </v-col>
        </v-row>
      </v-container>
    </div>
</template>

<script>
export default {
  name: 'NothingToShow',
  props: {
    title: String,
    message: String
  }
}
</script>

<style lang="scss" scoped>
.wrapper__without__content {
  opacity: 0.5;
  text-align: center;
  .text__without__content {
    color: #6600cc;
    text-transform: uppercase;
    font-size: 3.5em;
    font-weight: normal;
  }
}
.full__width {
  width: 100%;
}
.full__height {
  height: 90%;
}
</style>