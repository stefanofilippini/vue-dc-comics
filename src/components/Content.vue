<template>
    <div class="content">
        <div class="text-container">
            <span></span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Content'
}
</script>

<style lang="scss" scoped>

    .content {
        width: 100%;
        height: 120px;
        background-color: #1b1b1b;
        .text-container {
            display: flex;
            align-items: center;
            span {
                font-weight: 700;
                color: white;
                font-size: 24px;
                &::before {
                    content: '--> Content Goes Here <--';
                }
            }
        }
    }
</style>