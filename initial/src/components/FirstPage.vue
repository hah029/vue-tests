

<template>
    <div>
        
        <div class="row justify-content-md-center">
            <img 
                class="img-logo-class"
                src="../assets/IndexLogo.png"                
            >
        </div>

        <div class="row" style="margin-top: 44px;">
            <ul v-for="(card, index) in cards" :key="index"
                class="col">
                <main-card 
                    :title = "card.title"
                    :text = "card.text"
                    :lowerIndex = "card.lowerIndex"
                    class="card-active"
                    @click="clickEvent(index)"
                />
            </ul>
        </div>
        
    </div>
</template>


<script>
    import MainCard from './MainCard.vue'
    export default {
        name: 'MyNewPage',
        components: { MainCard },

        data() {
            return {
                cards: [
                    {
                        title: 'СИП',
                        text: 'Индекс готовности и интеграции проекта',
                        lowerIndex: '01',
                        active_: false
                    },
                    {
                        title: 'ОКС',
                        text: 'Аналитика процесса реализации объектов капитатльного строительства',
                        lowerIndex: '02',
                        active_: false
                    }
                ]
            }
        },
        methods: {
            clickEvent(index_) {
                alert(index_);
            }
        }
    }
</script>


<style lang="scss" scoped>
    .card {
        transition: 0.2s ease;
        &.backColor_ {
			background-color: #000000;
		}
    }
    .card-active:hover {
        border-color: rgb(0, 121, 194);
        background-color: rgb(236, 248, 255)
    }
    .img-logo-class {
        width: 162px;
        padding: 0;
    }
</style>