<svelte:options customElement="awc-input" />
<script>
    export let input_name, input_id;
    export let input_placeholder = 'Введите название';
    export let input_color;
</script>

<div>
  <input class="awc-input {input_color}" type="text" name={input_name} id={input_id}  placeholder={input_placeholder} />
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
  .red {
    background: red;
    color: white;
  }

  .purple {
    background: purple;
    color: white;
  }
</style>
