<template>
<div>
    <h1 v-Text> titulo </h1>
    <ul>
        <li v-for="foto of fotos">
            <p>{{foto.titulo}}</p>
            <img :src="foto.url" :alt="foto.titulo">
        </li>
    </ul>
</div>

</template>

<script>
export default{
    data() {
        return {
            titulo:'Text',
            fotos: [
            {
                url:'https://cdn.dicionariopopular.com/imagens/meme-da-mulher-gritando-com-o-gato-na-mesa-og.jpg',
                titulo: 'cachorro'
            },
            {
                url:'https://1.bp.blogspot.com/-Gg8gS6MIsEQ/XYEV3cSKEEI/AAAAAAABOH8/LCRbWmmmGXUpCO3G9L2JmFC6P36Ugn5zACLcBGAsYHQ/s1600/1%25271%25271%25271.jpg',
                titulo: 'Rau'
            }
        ]
        }
    }
}
</script>

<style>

</style>