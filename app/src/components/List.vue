<template>
<div>
    <div class="color">Lista</div>
    <div v-for="(obj, index) in todos" v-bind:key="obj.id">
      {{ index }} - {{obj.title }}
    </div>
    <!-- <div v-for="obj in todos" v-bind:key="obj.id">
        {{obj.title }}
    </div> -->
</div>
</template>

    
<script>
export default {
    name: 'One-List',
    props: {
        msg: String
    },

    data() {

        return {
            todos: [{
                    "userId": 1,
                    "id": 1,
                    "title": "zero",
                    "completed": false
                },
                {
                    "userId": 1,
                    "id": 2,
                    "title": "um",
                    "completed": false
                },
                {
                    "userId": 1,
                    "id": 3,
                    "title": "dois",
                    "completed": false
                },
                {
                    "userId": 1,
                    "id": 4,
                    "title": "tres",
                    "completed": false
                },
                {
                    "userId": 1,
                    "id": 5,
                    "title": "quatro",
                    "completed": false
                },
            ]
        }

    }
}
</script>

    
<style scoped>
.color{
color: green;
font-size: 20px;
}
</style>
