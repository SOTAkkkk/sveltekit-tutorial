<script>
    let count = 0;
    $: doubled = count * 2;

    function inclement() {
        count++;
    }
</script>

<button on:click={inclement}>
    Clicked {count}
    {count === 1 ? 'time' : 'times'}
</button>

<p>{count} doubled is {doubled}</p>