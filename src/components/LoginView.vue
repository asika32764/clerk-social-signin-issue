<script setup lang="ts">

import { SignIn, SignedIn, SignedOut } from '@clerk/vue';
</script>

<template>
<div>
  <SignedOut>
    <SignIn />
  </SignedOut>
  <SignedIn>
    Login Success!
  </SignedIn>
</div>
</template>

<style scoped>

</style>
