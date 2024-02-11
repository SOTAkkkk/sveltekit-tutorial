<script>
    let count = 0;

    function increment() {
        count++;
    }
</script>

<button on:click={increment}>
    Clicked {count}
    {count === 1 ? 'time' : 'times'}
</button>

{#if count > 10}
    <p>{count} is greater then 10</p>
{/if}