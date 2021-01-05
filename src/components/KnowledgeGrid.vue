<template>
  <ul>
    <knowledge-element
      v-for="topic in topicsProvide"
      :key="topic.id"
      :id="topic.id"
      :topic-name="topic.title"
      :description="topic.description"
    ></knowledge-element>
  </ul>
</template>

<script>
export default {
  inject:['topicsProvide'],
};
</script>