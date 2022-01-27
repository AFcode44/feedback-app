<script lang="ts">
    import type { CardDTO } from "../../model/card/card-dto";

    export let item: CardDTO;
</script>

<div class="__card-main-container">
    {item.message}
    <div class="__card-raiting-container">
        <span>{item.raiting}</span>
    </div>
</div>

<style lang="scss">
    .__card-main-container {
        display: flex;
        padding: 20px 50px;
        background: #fff;
        color: #333;
        border-radius: 15px;
        margin: 28px 0;
        position: relative;
    }

    .__card-raiting-container {
        position: absolute;
        top: -20px;
        left: -20px;
        background: #800b7e;
        border: 1px solid #fff;
        color: #fff;
        border-radius: 50%;
        height: 44px;
        width: 44px;
        display: flex;
        align-items: center;
        justify-content: center;

        span {
            margin-bottom: 4px;
            font-size: 1.3rem;
        }
    }
</style>
