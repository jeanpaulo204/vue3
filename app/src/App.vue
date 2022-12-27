<template>
<Header v-if="showHeader" />

<div v-show="ShowName">
    Nome:{{ FirstName }}
    <br />
    SobreNome:{{ LastName }}
</div>

<div v-if="accessLevel === 'admin'">Usuario: Admin</div>
<div v-else-if="accessLevel === 'marketing'">Usuario: Marketing</div>
<div v-else>Usuario: Normal</div>
<br/>
<Lista/>


</template>

<script>
import Header from './components/theHeader.vue'
import Lista from './components/List.vue'

export default {
    name: 'App',
    components: {
        Lista,
        Header
    },

    data() {

        return {
            showHeader: true,
            ShowName: false,
            FirstName: 'Bob Sponja',
            LastName: 'Calca Quadrada',
            accessLevel: 'admin'
        }

    }

}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
