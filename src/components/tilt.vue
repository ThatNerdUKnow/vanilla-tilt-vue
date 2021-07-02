<template>
    <div id="tiltMe" ref="testRef">
        <slot></slot>
        
    </div>
</template>

<script>
import VanillaTilt from 'vanilla-tilt';

export default {
    name: 'Tilt',
    data: function(){
        return {
        }
    },
    mounted(){
        
        VanillaTilt.init(this.$refs.testRef,this.options)
        
       
    },
    props: {
        options: Object
    }
}
</script>
