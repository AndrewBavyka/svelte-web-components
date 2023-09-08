<script>
  import Input from "./components/Input.svelte";
  import TabGroup from "./components/tabs/TabGroup.svelte";
  import Tab from "./components/tabs/Tab.svelte";
</script>

<main>
  <div class="block">
    <h2>Поля ввода</h2>
    <awc-input
      name="input-awc-1"
      color="red"
      placeholder="Вставьте ссылку 1"
      id="id-1"
    />
    <awc-input name="input-awc-2" color="purple" placeholder="Вставьте ссылку 2" id="id-2" />
  </div>
  <div class="block">
    <h2>Табы</h2>
    <awc-tab id="tab-1" name="Название таба" />
    <awc-tab id="tab-2" name="" />
  </div>
  <div class="block">
    <h2>Группы табов</h2>
    <awc-tab-group>
      <awc-tab id="tab-3" name="Общие" />
      <awc-tab id="tab-4" name="Транзакции" />
      <awc-tab id="tab-5" name="История" />
    </awc-tab-group>
  </div>
</main>
