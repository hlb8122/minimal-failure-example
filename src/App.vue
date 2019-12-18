<template>
  <div id="q-app">
    <router-view />
  </div>
</template>

<script>
var grpc = require('grpc')

export default {
  created () {
    grpc.getClientChannel() // This can be anything involving gRPC
  }
}
</script>
