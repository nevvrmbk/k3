<script lang="ts">
    let count: number = 0;
</script>

<section class="container text-center p-4">
    <h2 class="border-bottom">Counter</h2>
    <p class="lead">
        <button class="btn btn-dark btn-outline-success" on:click={() => {
            count = count + 1;
        }}>Count is { count }</button>
    </p>
</section>
