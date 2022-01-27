<script lang="ts">
import type { CardDTO } from "../../model/card/card-dto";
import Card from "./Card.svelte";

    export let items: Array<CardDTO>;
</script>

    {#each items as item}
        <Card {item}/>
    {/each}

<style>

</style>
