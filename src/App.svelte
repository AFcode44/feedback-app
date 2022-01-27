<script lang="ts">
import CardList from "./components/card/CardList.svelte";
import type { CardDTO } from "./model/card/card-dto";

	const testData: Array<CardDTO> = [
		{
			message: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Aperiam sapiente esse perferendis, saepe molestias minus facere consequuntur sint nam nostrum!',
			raiting: 9
		},
		{
			message: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam cum praesentium quae.',
			raiting: 5
		}
	];
</script>

<main>
	<div class="__main-container">
		<CardList items={testData}/>
	</div>
</main>

<style>
	.__main-container {
		width: 768px;
		margin: 0 auto;
	}
</style>