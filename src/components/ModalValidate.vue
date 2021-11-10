        <template>
            <modal 
                title="Modal with form" 
                @click="$emit('close')">

                <div slot="body">
                    <form @submit.prevent="submitSecondForm">
                        <label>Name:</label>
                        <input type="text" required v-model="modalSecond.name">
                        <label>Email:</label>
                        <input type="email" required v-model="modalSecond.Email">
                    <button class="btn btnPrimary">Submit</button>
                    </form>
                </div>
                </modal>
        </template>


<script>
import modal from '@/components/Modal.vue'
export default {
    components: {modal}
}
</script>
