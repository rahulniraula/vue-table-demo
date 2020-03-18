<template>
    <div>
        <v-table  :items="data" :except="['states']"/>
    </div>
</template>
<script>
import vTable from "geeklearners-vue-table";
export default {
    components:{vTable},
    data:function(){
        return {
            data:[]
        }
    },
    mounted:function(){
        fetch("https://raw.githubusercontent.com/stefanbinder/countries-states/master/countries.json")
        .then(resp=>resp.json())
        .then(data=>{this.data=data})

    }
}
</script>