<template>
    <main id="gallery-page">
        <h1>Gallery</h1>
        <p>This is the Gallery page</p>
        <!-- <img src="../assets/fruit-1.jpg"/> -->
        <div class="row">
            <div class="gallery">
                <div class="container">
                    <img v-for="(images, index) in images" :key="index" v-bind:src="'/src/assets/fruit-' + (index + 1) + '.jpg'"/>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
    export default {
        data() {
            return {
                images: [
                    {
                        idImage: 1,
                        image: "fruit-1.jpg"
                    },
                    {
                        idImage: 2,
                        image: "fruit-2.jpg"
                    },
                    {
                        idImage: 3,
                        image: "fruit-3.jpg"
                    },
                    {
                        idImage: 4,
                        image: "fruit-4.jpg"
                    },
                    {
                        idImage: 5,
                        image: "fruit-5.jpg"
                    },
                    {
                        idImage: 6,
                        image: "fruit-6.jpg"
                    },
                    {
                        idImage: 7,
                        image: "fruit-7.jpg"
                    },
                    {
                        idImage: 8,
                        image: "fruit-8.jpg"
                    },
                    {
                        idImage: 9,
                        image: "fruit-9.jpg"
                    },
                    {
                        idImage: 10,
                        image: "fruit-10.jpg"
                    },
                    {
                        idImage: 11,
                        image: "fruit-11.jpg"
                    },
                    {
                        idImage: 12,
                        image: "fruit-12.jpg"
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    main {
        margin-top: 120px;
        text-align: center;
    }
    .gallery {
        margin: 10rem;
    }
    .container {
        display: grid;
        grid-template-columns: repeat(4, 0.5fr);
        grid-gap: 1rem;
 
    }

    img {
        display: inline;
        width: 100%;
        height: 300px;
        margin: 1rem;
        object-fit: cover;
        object-position: center;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
    }
    
</style>