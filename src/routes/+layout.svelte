<script>
  import MyButton from "./Button.svelte";
  import "../app.css";
</script>

<svelte:head>
  <link
    rel="stylesheet"
    href="https://unpkg.com/tailwindcss@2.2.19/dist/tailwind.min.css"
  />
</svelte:head>
<body>
  <!-- SINGLE HTML BUTTON COMPONENT -->
  <div class="flex flex-col justify-center items-center h-screen m-auto">
    <div class="p-3">
      <MyButton name="Button" type="disabled"  />
    </div>
    <div class="p-3">
      <MyButton name="Button" type="flat" />
    </div>
    <div class="p-3">
      <MyButton name="Button" type="regular"/>
    </div>
  </div>
</body>
