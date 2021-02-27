<template>
    <div>
        子组件
        <!-- :data 是自定义属性？？？？ -->
        <slot  :data='data' />
    </div>
</template>
<script>
export default {
    name:"childTemplate",
    // props:['user'],
    data() {
        return {
            data:['MonDay','TuesDay','Wednesday','Thursday','Friday','Saturday','Sunday']
        }
    },
}
</script>