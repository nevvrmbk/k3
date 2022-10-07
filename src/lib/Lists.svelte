<script lang="ts">
    let items: string[] = [];
    let item: string = '';
</script>

<div class="container text-center">
    <fieldset>
        <legend>My List</legend>
    
        <form on:click|trusted|preventDefault={() => {
            if (item) {
                items = [...items, item];
                item = '';
            }
        }}>
            <label class="form-label">
                Item
                <input class="form-control form-control-lg" type="text" bind:value={ item } placeholder="Add on item to the list" />
            </label>
    
            <button type="submit" class="btn btn-outline-dark">Add</button>
        </form>
    
        <output>
            {#each items as item, i}
            <p>{ i } { item }</p>
            {:else}
            <p>No items found</p>
            {/each}
        </output>
    </fieldset>
</div>
