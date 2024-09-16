<script>
  export let name = "Button";
  export let type = "regular"; // regular, flat, disabled
  export let color = "purple";
  //export let size = "md"; // sm, md, lg
  //const sizes = {
  //  sm: "px-1 py-3 pr-8 pl-8",
  //  md: "px-5 py-3 pr-8 pl-8",
  // lg: "px-7 py-5 pr-8 pl-8",
  //};
</script>

{#if type == "regular"}
  <button
    class={`rounded-full py-3 px-5 pr-36 pl-36 bg-${color}-400 font-bold text-indigo-600`}
  >
    {name}
  </button>
{/if}

{#if type == "flat"}
  <button
    class={`rounded-full py-3 px-5 pr-36 pl-36 font-bold border border-2 border-none text-indigo-600 bg-${color}-200`}
  >
    {name}
  </button>
{/if}

{#if type == "disabled"}
  <button
    class={`rounded-full py-3 px-5 pr-36 pl-36 font-bold bg-gray-200 text-gray-400`}
  >
    {name}
  </button>
{/if}
