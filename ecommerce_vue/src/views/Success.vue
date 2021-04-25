<template>
    <div class="page-success">
        <div class="columns is-multiline">
            <div class="column is-12">
                <h1 class="title has-text-centered has-text-weight-bold has-text-medium">Thank you for your order!</h1>
                <p class="is-size-6 has-text-centered"> Your order will be processed and confirmed shortly.<br>If you have any questions, please feel free to contact us at (718) 292-5000</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Success',
    mounted() {
        document.title = 'Successfully Placed | Giant Food System, INC'
    },
}
</script>