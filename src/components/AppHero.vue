<script >
    export default {
        name: "AppHero",

        data() {
            return {
                message: "",
                img: "https://static.thenounproject.com/png/1913796-200.png",
                // l'img sta funzionando solo con l'url online, perchè?
            }
        },

        methods: {
            buttonTrigger() {
                this.message = "Absolutely Nothing is happening!";
            }
        },
    };

    
</script>

<template>
    
    <div id="jumbotron-container">
        <img :src="img" alt="PurpleTheJumbo" />
        <div id="jumbotron">
            <h2>
                A Friendly Purple Jumbotron
            </h2>
            <p>
                Jumbotron it's a really big and funny section. Like a very big board! <br>
                You can also add a button to make your Friendly Purple Jumbotron <br>
                more friendly!
            </p>
            <button @click="buttonTrigger()">
                Click me!
            </button>
            {{ message }}
        </div>
        <img :src="img" alt="PurpleTheJumbo" />
    </div>

</template>

<style >
    #jumbotron-container {
        margin-top: 1em;
        border: 1px solid white;

        display: flex;
        justify-content: center;

        background-color: rgba(137, 43, 226, 0.459);
    }

    #jumbotron {
        display: flex;
        flex-direction: column;
        align-items: center;

        text-align: center;
        margin: 1em;

        border: 1px solid white;
        padding: 2em 2em;

        background-color: blueviolet;
    }

    button {
        color: blueviolet;
        background-color: whitesmoke;

        border: none;
        border-radius: 12px;
        margin: 1em 0em;
        padding: 1em;

        cursor: pointer;
    }

    img {
        height: 200px;
        align-self: center;
    }
</style>