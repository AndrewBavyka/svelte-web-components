<svelte:options customElement="awc-tab-group" />

<div class="tab-group">
    <slot></slot>
</div>

<style>
    .tab-group {
    max-width: max-content;
    display: flex;
    align-items: center;
    gap: 34px;
    padding-bottom: 12px;
    border-bottom: 1px solid var(--secondary-text);
}
</style>