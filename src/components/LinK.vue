<template>
    <li>
        <a
            :href="link"
            target="_blank"
            rel="smth"
        >
            <span class="button_icon">
            <img
                :src="image"
                alt="Not found"
            /> </span
            ><span class="button_text">{{ web }}</span>
        </a>       
    </li>

</template>

<script setup>

// PROPS
defineProps({
    link: {
        type: String,
        required: true
    },
    image: {
        type: String,
        required: true
    },
    web: {
        type: String, 
        required: true
    }
})
</script>