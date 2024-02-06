<template>
    <div
        class="mb-3 entry-container pointer p-2"
        @click="$router.push({ name: 'entry', params: { id: 10 } })"
    >
        <div class="entry-title d-flex">
            <span class="text-success fs-5 fw-bold">02</span>
            <span class="mx-1 fs-5">Febrero</span>
            <span class="mx-2 fw-light">2024, Viernes</span>
        </div>
        <div class="entry-description">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Beatae
            repudiandae perspiciatis tempore. Nesciunt a expedita, laboriosam
            dignissimos commodi alias, molestias quasi omnis quo nemo ullam
            similique repellat dolorem perspiciatis aperiam?
        </div>
    </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.entry-container {
    border-bottom: 1px solid #2c3e50;
    transition: 0.2s ease-in;
    &:hover {
        background-color: lighten($color: grey, $amount: 45);
        transition: 0.2 all ease-in;
    }
    .entry-description {
        font-size: 12px;
    }
}
</style>
