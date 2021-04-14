<template>
    <div>
        <button @click="incrementCount">Clicked {{ count }} times </button>
    </div>
</template>

<script>
import myMixin from '../mixins/myMixin'
export default {
name: 'ClickCounter',
mixins: [myMixin],
}
</script>