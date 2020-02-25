<template>
  <div class="hello">
    <button v-on:click="vanillaJS()">button</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  methods: {
    vanillaJS() {
      var arr1 = ["a", "b", "c"];
      var unorderedList = document.createElement("ul");
      unorderedList.style.cssText =
        "background:tomato; width: 400px;height:400px";
      document.body.appendChild(unorderedList);
      for (var i = 0; i < 3; i++) {
        var listItem = document.createElement("li");
        listItem.className = "list-item";
        unorderedList.appendChild(listItem);
        listItem.innerHTML = arr1[i];
      }
    }
  }
};
</script>
