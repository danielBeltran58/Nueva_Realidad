<script setup>
    const props = defineProps({
        title: String,
        nameChecked: String,
        radioOptions: Array
    });
</script>

<template>
    <p class="mb-0">{{ title }}</p>
    <div
    v-for="i in radioOptions"
    >
        <div class="form-check">
            <input class="form-check-input" type="radio" :name="nameChecked" :id="'flexRadioDefault' + radioOptions.indexOf(i)">
            <label class="form-check-label" :for="'flexRadioDefault' + radioOptions.indexOf(i)">
                {{ i }}
            </label>
        </div>
    </div>
</template>