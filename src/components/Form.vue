<template>
    <div class="form">
        <div class="form--content">
            <div class="form-nav--box">
                <i class="fal fa-arrow-left"></i>
                <h2 class="form-nav--header">Add something new</h2>
            </div>
            <i class="fad fa-clipboard-list form--icon"></i>

            <div class="form-input--box">
                <select class="form-input--select" v-model="formData">
                    <option v-for="category in categories" :key="category">{{ category.item }}</option>
                </select>

                <div class="form-input--item">
                    <input type="text" placeholder="Name" class="form-input--text" />
                    <i class="fal fa-times"></i>
                </div>
            </div>
            <!-- <button @click="getInput()">Click me</button> -->
        </div>
    </div>
</template>

<script>
    export default {
        data: function () {
            return {
                categories: [{
                        item: 'Business'
                    },
                    {
                        item: 'Meeting'
                    },
                    {
                        item: 'Home'
                    },
                    {
                        item: 'Sport'
                    }
                ],
                formData: ''
            }
        },

        methods: {
            getInput() {
                this
            }
        }
    }
</script>