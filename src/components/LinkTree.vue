<template>
    <div>
        <div class="linktree_container">
          <ul class="linktree">
            <LinK
                :link="links.youtube.link"
                :image="links.youtube.image"
                :web="links.youtube.web"
            />
            <LinK
                :link="links.facebook.link"
                :image="links.facebook.image"
                :web="links.facebook.web"
            />
            <LinK
                :link="links.ig.link"
                :image="links.ig.image"
                :web="links.ig.web"
            />
            <LinK
                :link="links.spotify.link"
                :image="links.spotify.image"
                :web="links.spotify.web"
            />
            <LinK
                :link="links.linkedin.link"
                :image="links.linkedin.image"
                :web="links.linkedin.web"
            />
            <LinK
                :link="links.tiktok.link"
                :image="links.tiktok.image"
                :web="links.tiktok.web"
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

const links = reactive({
    youtube: {
        link: "https://www.youtube.com/tomipvideos",
        image: "/src/imgs/Youtube Icon.jpg",
        web: "Youtube"
    },
    facebook: {
        link: "https://www.facebook.com/TomiPVideos",
        image: "/src/imgs/Facebook Icon.jpg",
        web: "Facebook"
    },
    ig: {
        link: "https://www.instagram.com/tomipizur/",
        image: "/src/imgs/Instagram Icon.jpg",
        web: "Instagram"
    },
    spotify: {
        link: "https://open.spotify.com/artist/525zfSkeWFp2fd2zf2CwOD?si=K22wymtISISCGCTFJIMxcA",
        image: "/src/imgs/Spotify Icon.jpg",
        web: "Spotify"
    },
    linkedin: {
        link: "https://www.linkedin.com/in/tom%C3%A1%C5%A1-piz%C3%BAr-39838724b/",
        image: "/src/imgs/LinkedIn Icon.jpg",
        web: "LinkedIn"
    },
    tiktok: {
        link: "https://www.tiktok.com/@tomipmusic",
        image: "/src/imgs/TikTok Icon.jpg",
        web: "TikTok"
    },
})
</script>

<style>
.linktree{
    display: flex;
    gap: 10px;
    flex-direction: column;
    padding: 0;
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
    width: 50px;
    height: 50px;
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
</style>