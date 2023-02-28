

<template>


    <!-- <div class="container-fluid">
        <div class="row justify-content-md-center">
            <div class="col-11 test1">1</div>
            <div class="col test2">2</div>  
            <div class="col test3">3</div>  
        </div>
    </div> -->

    <div class="container-fluid">
        <div class="row justify-content-md-center">
            <div class="col test1">1</div>
        </div>
        <div class="row justify-content-md-center">
            <div class="col test2">1</div>
            <div class="col test2">2</div>  
            <div class="col test3">3</div> 
        </div>
    </div>

    <!-- <table class="table" style="display: flexbox;">
        <col style="width:50%;"/>
        <col style="width:40%;"/>
        <col style="width:10%;"/>
        <thead>
            <tr>
                <th>50</th>
                <th>40</th>
                <th>10</th>
            </tr>
        </thead>
    </table> -->
    

</template>


<script>
    export default {
        name: 'SecondPage',
        data() {
            return {
                test: 'Вторая страница'
            }
        }
    }
</script>


<style lang="scss" scoped>
    .test1 {
        background-color: burlywood;
        column-width: 64px;
    }
    .test2 {
        background-color:aquamarine;
    }
    .test3 {
        background-color:red;
    }
</style>