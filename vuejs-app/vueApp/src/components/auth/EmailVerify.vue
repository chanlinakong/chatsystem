<script setup>
import { onMounted } from "vue";
import axios from "axios";

onMounted(() => {
    const params = new URLSearchParams(window.location.search);

    const url = params.get("forwarded-url");

    if (url) {
        window.location.href = url;
    }
});
</script>

<template>
    <div>
        Verifying your email...
    </div>
</template>