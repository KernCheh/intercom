<template>
  <div class="md-layout md-gutter md-alignment-top-center">
    <!-- <md-button v-for="client in clients" :key="client.id" class="md-primary md-raised">
      {{ client.name }}
    </md-button> -->

    <section>
      <h1>
        Connected Clients:
      </h1>

      <md-list>
        <md-list-item>
          <md-avatar>
            <img src="https://placeimg.com/40/40/people/5" alt="People">
          </md-avatar>

          <span class="md-list-item-text">Abbey Christansen</span>

          <md-button class="md-icon-button md-list-action">
            <md-icon class="md-primary">
              chat_bubble
            </md-icon>
          </md-button>
        </md-list-item>
      </md-list>
    </section>
    <section />
  </div>
</template>

<script>
export default {
  data () {
    return {
      clients: [
        {
          id: 1,
          name: 'Living Room'
        },
        {
          id: 2,
          name: 'Kitchen'
        }
      ]
    }
  },

  mounted () {
    this.getClients()
  },

  methods: {
    getClients () {
      console.log('attempting to get clients')
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
