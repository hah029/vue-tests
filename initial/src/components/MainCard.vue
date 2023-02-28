

<template>
    <div class="card">
        <h5 
            class="card-title font-common-text"
            style="font-size: 64px"
        >{{ title }}</h5>

        <div class="row">
            <div class="col">
                <div 
                    class="font-common-text bottom-text"
                    style="font-size: 24px; width: 342px;"
                >{{ text }}</div>
            </div>
            
            <div class="col">
                <div 
                    class="col font-common-text bottom-text"
                    style="font-size: 32px; opacity: 30%; right: 42px;"
                >{{ lowerIndex }}</div>
            </div>
        </div>
    </div>
</template>


<script>
    export default {
        name: 'MainCard',
        props: { 
            title: String, 
            text: String, 
            lowerIndex: String 
        }
    }
</script>


<style>
    .card {
        margin: 0px;
        padding-left: 42px;
        padding-top: 32px;
        border-radius: 28px;
        width: 540px;
        height: 268px;
        border-width: 2px;
        border-color: #FFFFFF;
        box-shadow: 0px 4px 18px 0px rgba(219, 219, 219);
    }
    .card_hovered {
        background-color: #020202;
    }

    @font-face {
        font-family: 'sf-ui-display';
        src: url('../fonts/sf-ui-display-medium-58646be638f96.otf')
    }
    .font-common-text {
        font-family: 'sf-ui-display';
        color: #000000;
    }
    .bottom-text {
        position: absolute;
        bottom: 32px;
        line-height: 1
    }
</style>