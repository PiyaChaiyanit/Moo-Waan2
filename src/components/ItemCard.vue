<template>
    <div class="block container">
        <div class="is-multiline columns">

            <!-- Card element start here------------------------------------------>
            <div class="column is-one-quarter" v-for="(todo, index) in item" :key="index">
                <div class="card">
                    <div class="card-image">
                        <figure class="image is-1by1">
                            <img src="https://bulma.io/images/placeholders/640x480.png" alt="Placeholder image">
                        </figure>
                    </div>
                    <div class="card-content">
                        <div class="media">
                            <div class="media-content">
                                <p class="title is-4">{{ todo.name }}</p>
                                <p class="has-text-left">ชนิด : {{ todo.type }}</p>
                                <p class="has-text-left">ราคา : {{ todo.price }} ฿</p>
                            </div>
                        </div>
                        <div class="has-text-right">
                            <router-link to="/SelectedItems" class="button is-rounded">
                                Select
                            </router-link>
                        </div>

                    </div>
                </div>
            </div>

        </div>
    </div>
</template>

<style>
@import "https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css";
</style>

<script>
import item from "../item.json"



export default {
    name: 'SignUpPage',
    props: {
        msg: String
    },
    data() {
        return {
            item,
            cart: [],
        }
    }
}
</script>