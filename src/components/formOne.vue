<template>
    <div>
        <form-helper>
            <div slot="form-header">
                <header-one />
            </div>
            <div slot="form-fields">
                <input type="text" placeholder="name" required />
                <label>Your Message:</label>
                <textarea></textarea>
            </div>
            <div slot="form-controls">
                <button v-on:click="handleSubmit">Send</button>
            </div>
        </form-helper>
    </div>
</template>

<script>
// Imports
import formHelper from './formHelper.vue'
import HeaderOne from './headerFormOne.vue'

export default {
    components: {
        'form-helper': formHelper,
        'header-one': HeaderOne

    },
    data () {
        return {

        }
    },
    methods: {
        handleSubmit: function(){
            alert('thanks for submitting form one & contacting us');
        }
    }
}
</script>

<style>
body{
    margin: 0;
    font-family: 'Nunito SemiBold';
}
</style>
