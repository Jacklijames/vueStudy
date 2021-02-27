<template>
    <div>
        <child-template>
            <template slot-scope="slotProps">
                <ul>
                    <li v-for="(item, index) in slotProps.data" :key="index">
                        {{item}}
                    </li>
                </ul>
            </template>
        </child-template>
    </div>
</template>
<script>

// 导入子组件
import {childTemplate} from './child'

export default {
  components: { childTemplate },
    name:"parentTempt"
    
}
</script>