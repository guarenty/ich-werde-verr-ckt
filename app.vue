<template>
  {{ data }}
</template>

<script setup lang="ts">
const supabase = useSupabaseClient()

const { data, error } = await supabase.auth.signInWithPassword({
  email: "tester@test.de",
  password: "password"
})
</script>