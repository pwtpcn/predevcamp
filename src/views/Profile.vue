<template>
    <div>
        <profileCard v-for="member in members" :key="member"
        :image="member.image"
        :name = "member.name"
        :study = "member.study"
        :birthday = "member.birthday"/>
    </div>
</template>

<script>
import profileCard from "../components/Profile.vue"
export default{
    data(){
        return{
            members:[
                {
                    name: "Thanapoom Chaisena",
                    birthday: "23 Jan 2004",
                    study: "KU82 CS37",
                    image: "../assets/IMG_20220430_224331_058.jpg"
                },
                {
                    name:"Kritt Wongwandee",
                    birthday:"29 Aug 2003",
                    study: "KU82 CS37"
                },
                {
                    name:"Harit Sombatsiri",
                    birthday:"24 Nov 2003",
                    study: "KU82 CS37"
                }
            ],
            
        }
    },
    components:{
        profileCard,
    },
};
</script>


<style>

</style>