<svelte:options
  customElement={{
    tag: 'awc-input',
    props: {
      color: { reflect: true, type: 'String', attribute: 'color-input' },
    },
  }}
/>

<script>
  export let input_name;
  export let input_id;
  export let placeholder = 'Введите название';
  export let color = 'default'; 
</script>

<div>
  <input
    class="awc-input {color}"
    type="text"
    name={input_name}
    id={input_id}
    placeholder={placeholder}
  />
</div>

<style>
  .awc-input {
    padding: 13px 0 13px 16px;
    border-radius: 5px;
    border: none;
    color: var(--secondary-text);
    background: var(--input-background);
  }

  .awc-input:focus-visible {
    outline: 1px solid var(--secondary-text);
  }

  .awc-input.default {
    background: var(--input-background);
    color: var(--secondary-text);
  }

  .awc-input.red {
    background: red;
    color: white;
  }

  .awc-input.purple {
    background: purple;
    color: white;
  }
</style>
