<template>
    <div>
        <div class="linktree_container">
          <ul class="linktree">
            <LinK
                v-for="website in links"
                :key="website.web"
                :link="website.link"
                :image="website.image"
                :web="website.web"
            />
          </ul>
        </div>
        <FormContainer/>
    </div>
</template>

<script setup>
    import FormContainer from '@/components/FormContainer.vue'
    import LinK from '@/components/LinK.vue'
    import { reactive } from 'vue'

const links = [
    {
        link: "https://www.youtube.com/tomipvideos",
        image: "/src/imgs/Youtube.png",
        web: "Youtube"
    },
    {
        link: "https://www.facebook.com/TomiPVideos",
        image: "/src/imgs/Facebook.png",
        web: "Facebook"
    },
    {
        link: "https://www.instagram.com/tomipizur/",
        image: "/src/imgs/Instagram.png",
        web: "Instagram"
    },
    {
        link: "https://open.spotify.com/artist/525zfSkeWFp2fd2zf2CwOD?si=K22wymtISISCGCTFJIMxcA",
        image: "/src/imgs/Spotify.png",
        web: "Spotify"
    },
    {
        link: "https://www.linkedin.com/in/tom%C3%A1%C5%A1-piz%C3%BAr-39838724b/",
        image: "/src/imgs/LinkedIn.png",
        web: "LinkedIn"
    },
    {
        link: "https://www.tiktok.com/@tomipmusic",
        image: "/src/imgs/TikTok.png",
        web: "TikTok"
    },
]
</script>

<style>
.linktree_container{
    display: flex;
    justify-content: center;
}
.linktree{
    display: flex;
    gap: 10px;
    flex-direction: column;
    padding: 0;
    width: 80%;
}
li{
    list-style-type: none;
    margin: 0;
}

.linktree li a {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 2em;
    background-color: rgb(255, 255, 255);
    padding: 14px 80px;
    transition: background 400ms;
    text-decoration: none;
    color: black;
    font-weight: bold;
    font-size: 30px;
}

.button_icon{
    display: flex;
    width: 60px;
    height: 60px;
    align-content: center;
    border: 2px solid rgb(170, 170, 170);
    border-radius: 30%;
    margin-right: 20px;
}

.button_text{
    width: 5em;
    text-align: left;
}
.button_icon img{
    border-radius: 30%;
}

.linktree li a:hover{
    background-color: rgb(170, 170, 170);
}

@media (max-width: 1221px) {
    .linktree{
    width: 87%;
}
}
@media (max-width: 667px) {
    .linktree{
    width: 100%;
}
}
</style>