<template>
       <div
      class="grey lighten-3"
       >
    <v-card>
 <v-layout>
    <v-flex xs12 sm6 offset-sm3>
      <v-card>
        <v-card-media src="/static/doc-images/cards/desert.jpg" height="200px">
        </v-card-media>
        <v-card-title primary-title>
          <div>
            <h3 class="headline mb-0">{{title}}</h3>
            <div>{{description}} <br>
            {{reason}}</div>
          </div>
        </v-card-title>
        <slot></slot>
        </v-card>
      </v-flex>
  </v-layout>
    </v-card>
  </div>    

</template>

<script>
export default {
  props: ['title', 'reason', 'description'],
};
</script>