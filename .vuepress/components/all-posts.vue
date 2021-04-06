<template>
  <div>
    <p v-for="post in $site.pages.filter(p => p.path.includes('/that'))">
      <router-link :to="post.path">{{ post.title }}</router-link>
    </p>
  </div>
</template>