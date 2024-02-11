<script>
    let count = 0;
    $: {
        console.log(`the count is ${count}`);
        console.log(`this will alos logged whenever count changes`)
    }
    $: if (count >= 10) {
        alert(`count is dangerously high!`);
        count = 0;
    }

    function inclement() {
        count++;
    }
</script>

<button on:click={inclement}>
    Clicked {count}
    {count === 1 ? 'time' : 'times'}
</button>
