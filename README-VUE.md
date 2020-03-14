
<!DOCTYPE html>
<html>
<head>
  <title>Toggle Message</title>
  <script src="https://cdn.jsdelivr.net/npm/vue@2.6.10/dist/vue.min.js"></script>
</head>
<body>
  <div id="app">
    <!-- Add missing attributes to a and p elements -->
    <a href="#" v-on:click="isVisible = !isVisible">Want to buy a new car?</a>
    <p v-if="isVisible">Call +11 22 33 44 now!</p>
  </div>
  <script>
    var vm = new Vue({
        el: '#app',
        data: {
          isVisible: false
        }
      });
    
    // Example case
    console.log(document.getElementById("app").innerHTML);
  </script>
</body>
</html>
