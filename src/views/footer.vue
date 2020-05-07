<template>
        <footer>
            <div id="social-links">
                <ul>
                    <li>
                        <v-btn text small target="_blank" href="https://www.instagram.com/gerdurdesign">
                        <v-icon id="icon">fab fa-instagram</v-icon>
                            Instagram
                        </v-btn>
                    </li>
                    <li>
                        <v-btn text small target="_blank" href="https://www.linkedin.com/in/thorgerdur/">
                        <v-icon id="icon">fab fa-linkedin</v-icon>
                            LinkedIn
                        </v-btn>
                    </li>
                </ul>
            </div>
        </footer>
</template>




<script>
    export default {
      
    }
</script>

<style scoped>
    footer {
        background-color: rgb(236, 236, 236);
        width: 100%;
        height: 80px;
    }

    ul {
    list-style: none;
    margin: 10px;
    margin-left: -20px;
    }

    #icon {
        margin: 10px;
    }
</style>