<template>
  <div>
    <h1>Latest News</h1>

    <ol>
      <li v-bind:key="blog.id" v-for="blog in blogs">
        {{ blog.title }}
        <p>{{ blog.content }}</p>
      </li>
    </ol>
</div>
</template>

<script>
export default {
  name: 'Blogs',
  data:function() {
    return  {
      blogs:
        [{

          id: 1,
          title: "First Blog",
          content: "About Vue"
        },
        {
          id: 2,
          title: "First Blog",
          content: "About Vue"
        },
        {
          id: 3,
          title: "First Blog",
          content: "About Vue"
        }]
    }
  }
}
</script>
