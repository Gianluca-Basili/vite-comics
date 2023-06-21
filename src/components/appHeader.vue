<script>
export default {
    data() {
        return {
            links:[
                {
                    label:'CHARACTERS',
                    href:'#',
                    active: false

                },
                {
                    label:'COMICS',
                    href:'#',
                    active: true

                },
                {
                    label:'MOVIES',
                    href:'#',
                    active: false

                },
                {
                    label:'TV',
                    href:'#',
                    active: false

                },
                {
                    label:'GAMES',
                    href:'#',
                    active: false

                },
                {
                    label:'COLLECTIBLES',
                    href:'#',
                    active: false

                },
                {
                    label:'VIDEOS',
                    href:'#',
                    active: false

                },
                {
                    label:'FANS',
                    href:'#',
                    active: false

                },
                {
                    label:'NEWS',
                    href:'#',
                    active: false

                },
                {
                    label:'SHOP',
                    href:'#',
                    active: false

                }

            ]
        }
    },
}
</script>
<template lang="">
    <header class="container">
        <div class="flex justify-between align-center">
            <a href="/">
                <img src="../assets/img/dc-logo.png">
            </a>
            <ul>
                <li v-for="(link, index) in links" :key="index " :active="link.active ? 'active' : ''">
                    <a :href="link.href" >
                        {{link.label}}
                    </a>
                </li>
    
            </ul>

        </div>
    </header>
</template>
<style lang="scss" scoped>

    .active{
        border-bottom: 3px solid blue;
    }

    header{
        padding: 20px 0px;
        height: 40px;
        
       ul li {
            display: inline-block;
            padding: 0px 20px;
            height: 40px;
            border-bottom: 5px solid white;

            a{
                font-size: 12px;
                font-weight: 600;
            }

            &:hover{
                border-bottom: 3px solid blue;
            }
        }
    }
</style>