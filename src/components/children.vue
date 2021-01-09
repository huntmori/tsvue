<template>
    <div>
        {{message}}
    </div>
</template>

<script lang="ts">
    import {Component, Prop, Vue, Watch, Emit, Inject} from 'vue-property-decorator';

    @Component export default class Children extends Vue{
        @Inject() readonly message!: string;
    }
</script>
