<template>
    <h2>Esta é a descrição da pessoa: </h2>
   <Info/>
   <Form/>
    
</template>

<script>
import Info from './Info';
import Form from './Form';

export default {
    name: 'Pessoa',
    components: {
        Info,
        Form
    },
    data() {
        return {
            nome: 'Vinicius'
        }
    }
}
</script>