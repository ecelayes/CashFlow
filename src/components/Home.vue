<template>
    <Layout>
        <template #header>
            <Header />
        </template>
        <template #resume>
            <Resume
                :label="'Ahorro Total'"
                :totalAmount="100000"
                :amount="1000"
            >
                <template #graphic>graphic</template>
                <template #action>action</template>
            </Resume>
        </template>
        <template #movements>
            <Movements />
        </template>
    </Layout>
</template>

<script>
import Layout from './Layout.vue'
import Header from './Header.vue'
import Resume from './Resume/Index.vue'
import Movements from './Movements.vue'

export default {
    components: {
        Layout,
        Header,
        Resume,
        Movements,
    },
}
</script>
