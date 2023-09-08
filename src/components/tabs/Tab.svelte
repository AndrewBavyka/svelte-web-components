<svelte:options
  customElement={{
    tag: 'awc-tab',
    props: {
      name: { reflect: true, type: 'String', attribute: 'text-in-tab' },
    },
  }}
/>

<script>
  export let name;
  export let tab_id = "Таб";
</script>

<div class="tab" id={tab_id}>
  {name || "Таб"}
  <slot />
  <span class="underline" />
</div>

<style>
  .tab {
    cursor: pointer;
    max-width: max-content;
    position: relative;
    border-radius: 5px;
    color: var(--secondary-text);
  }

  .tab:hover {
    transition: color 0.3s;
    color: var(--black-text);
  }

  .tab:hover .underline {
    width: 100%;
  }

  .underline {
    width: 0;
    height: 2px;
    background-color: var(--base-color);
    position: absolute;
    bottom: -12px;
    left: 0;
    transition: width 0.3s ease-in-out;
  }
</style>
