<template>
    <UButton :class="['flex items-center justify-center p-4 rounded-[35px] font-graphik-regular text-xl leading-0.5', 
    variants[props.variant],
    props.isBold ? 'font-graphik-bold': 'font-graphik-regular']">
        <slot></slot>
    </UButton>
</template>

<script setup>
const props = defineProps({
    variant: {
        type: String,
        default: 'default'
    },

    isBold: {
        type:Boolean,
        default: false
    }

})

const variants = {
    default: 'bg-white text-primary',
    primary: 'bg-primary text-white'
}


</script>