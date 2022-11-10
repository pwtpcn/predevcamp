<template>
    <div class="h-14 bg-gradient-to-r from-red-500 to-black flex justify-center items-center h-screen">
    <div class="min-h-screen flex justify-center items-center">
        <div class="w-96 h-128 rounded-xl bg-gray-200 flex flex-col">
            <img class = "w-auto rounded-t-xl" src="../assets/chrome_2021-11-22_20-48-54.png" alt="profile"/>
            <!-- <div class="h-32 w-32 bg-cover bg-center bg-no-repeat" :style="getUrlImage(image)"></div> -->
            <div class = "text-center flex flex-col p-2">
                <span class="text-base font-bold">{{name}}</span>
                <span class="text-base">{{study}}</span>
                <span class="text-xs">{{birthday}}</span>
            </div>
        </div>
    </div>
    </div>
</template>

<script>
    export default{
        props:{
            name:{
                type: String,
                default: "---"
            },
            study:{
                type: String,
                default: "---"
            },
            birthday:{
                type: String,
                default: "---"
            },
            image:{
                type: String,
                default:"../assets/chrome_2021-11-22_20-48-54.png"
            }
        },
    method:{
        getUrlImage(imagePath)
        {
            return ({ 'backgroung-image': 'url("./src/'+ imagePath +'")'});
        },
    }
    };
</script>

<style>
</style>