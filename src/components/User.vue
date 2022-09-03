<template>
    <div>
      <span className="user">
            <span className="name"> {{ user.name }}</span>
            <span className="handle">@{{ user.handle }}</span>
          </span>
    </div>
  </template>
  

<script>
export default {
    props: ["user"],
}
</script>

<style>

</style>