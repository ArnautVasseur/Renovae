<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
    <div class="mx-7">
        <h1 class="font-bold text-lg mt-10 mb-5">Recherche d'articles</h1>
        <SearchBar class="mb-5"/>
        <div class="mb-2 flex justify-between">
            <h2 class="font-bold text-lg">Pour toi</h2>
            <p class="text-orange">Voir d'autres objets</p>
        </div>
        <div class="grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(320px,320px))] justify-around mb-5">
            <a href="achat">
                <Card class="mb-5"
                image="/images/velo-wall-blue.png"
                :distance="27"
                state="Neuf"
                brand="SuperVelo"
                description="Vélo bleu neuf acheté il y a quelques mois."
                :price="30"
                :renovation="false"
                title="Vélo bleu"
                pp="/images/balland.png"
                :followers="419"
                :star1="true"
                :star2="true"
                :star3="true"
                :star4="true"
                :star5="false"
                :heart="true"
                name="Russel766"/>
            </a>
            <a href="achat">
                <Card
                image="/images/velo-wall-white.png"
                :distance="15"
                state="Rouillé"
                brand="Bikes"
                description="Vieux vélo inutilisable rouillé mais pouvant servir pour une rénovation."
                :price="22"
                :renovation="true"
                title="Velo marron"
                pp="/images/balland.png"
                :followers="142"
                :star1="true"
                :star2="true"
                :star3="false"
                :star4="false"
                :star5="false"
                :heart="false"
                name="Gertude"/>
            </a>
        </div>
        <h2 class="w-2/3 font-bold text-lg mb-3">Profils qui pourrait vous intéresser</h2>
        <a href="profil">
        <div class="mb-10 border-2 rounded-xl border-orange hover:border-4 p-5 flex">
            <div class="flex flex-col mr-4">
                <img src="../../public/images/balland.png" alt="Russel" class="w-16">
                <div class="flex ml-3 mt-1 pb-3 -mb-1">
                <svg width="7" height="7" viewBox="0 0 7 7" fill="none" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none">
                    <path
                        d="M3.05396 0.93275C3.29636 0.420529 3.9967 0.420528 4.2391 0.932749L4.65801 1.818C4.75427 2.0214 4.94033 2.16238 5.15556 2.195L6.09228 2.33696C6.63428 2.4191 6.8507 3.11376 6.45851 3.51247L5.78069 4.20154C5.62494 4.35986 5.55388 4.58798 5.59064 4.81154L5.75065 5.78452C5.84324 6.34751 5.27664 6.77683 4.79186 6.51103L3.95403 6.05165C3.76152 5.94609 3.53154 5.94609 3.33903 6.05165L2.5012 6.51103C2.01642 6.77683 1.44982 6.34751 1.54241 5.78452L1.70242 4.81154C1.73918 4.58798 1.66812 4.35986 1.51237 4.20154L0.834555 3.51247C0.442357 3.11376 0.658775 2.4191 1.20078 2.33696L2.1375 2.195C2.35273 2.16238 2.53879 2.0214 2.63505 1.818L3.05396 0.93275Z"
                        stroke="#EAB270"
                        stroke-width="0.40585"
                        stroke-linejoin="round"
                        class="fill-orange"
                    ></path>
                </svg>

                <svg width="7" height="7" viewBox="0 0 7 7" fill="none" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none">
                    <path
                        d="M3.05396 0.93275C3.29636 0.420529 3.9967 0.420528 4.2391 0.932749L4.65801 1.818C4.75427 2.0214 4.94033 2.16238 5.15556 2.195L6.09228 2.33696C6.63428 2.4191 6.8507 3.11376 6.45851 3.51247L5.78069 4.20154C5.62494 4.35986 5.55388 4.58798 5.59064 4.81154L5.75065 5.78452C5.84324 6.34751 5.27664 6.77683 4.79186 6.51103L3.95403 6.05165C3.76152 5.94609 3.53154 5.94609 3.33903 6.05165L2.5012 6.51103C2.01642 6.77683 1.44982 6.34751 1.54241 5.78452L1.70242 4.81154C1.73918 4.58798 1.66812 4.35986 1.51237 4.20154L0.834555 3.51247C0.442357 3.11376 0.658775 2.4191 1.20078 2.33696L2.1375 2.195C2.35273 2.16238 2.53879 2.0214 2.63505 1.818L3.05396 0.93275Z"
                        stroke="#EAB270"
                        stroke-width="0.40585"
                        stroke-linejoin="round"
                        class="fill-orange"
                    ></path>
                </svg>

                <svg width="7" height="7" viewBox="0 0 7 7" fill="none" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none">
                    <path
                        d="M3.05396 0.93275C3.29636 0.420529 3.9967 0.420528 4.2391 0.932749L4.65801 1.818C4.75427 2.0214 4.94033 2.16238 5.15556 2.195L6.09228 2.33696C6.63428 2.4191 6.8507 3.11376 6.45851 3.51247L5.78069 4.20154C5.62494 4.35986 5.55388 4.58798 5.59064 4.81154L5.75065 5.78452C5.84324 6.34751 5.27664 6.77683 4.79186 6.51103L3.95403 6.05165C3.76152 5.94609 3.53154 5.94609 3.33903 6.05165L2.5012 6.51103C2.01642 6.77683 1.44982 6.34751 1.54241 5.78452L1.70242 4.81154C1.73918 4.58798 1.66812 4.35986 1.51237 4.20154L0.834555 3.51247C0.442357 3.11376 0.658775 2.4191 1.20078 2.33696L2.1375 2.195C2.35273 2.16238 2.53879 2.0214 2.63505 1.818L3.05396 0.93275Z"
                        stroke="#EAB270"
                        stroke-width="0.40585"
                        stroke-linejoin="round"
                        class="fill-orange"
                    ></path>
                </svg>

                <svg width="7" height="7" viewBox="0 0 7 7" fill="none" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none">
                    <path
                        d="M3.05396 0.93275C3.29636 0.420529 3.9967 0.420528 4.2391 0.932749L4.65801 1.818C4.75427 2.0214 4.94033 2.16238 5.15556 2.195L6.09228 2.33696C6.63428 2.4191 6.8507 3.11376 6.45851 3.51247L5.78069 4.20154C5.62494 4.35986 5.55388 4.58798 5.59064 4.81154L5.75065 5.78452C5.84324 6.34751 5.27664 6.77683 4.79186 6.51103L3.95403 6.05165C3.76152 5.94609 3.53154 5.94609 3.33903 6.05165L2.5012 6.51103C2.01642 6.77683 1.44982 6.34751 1.54241 5.78452L1.70242 4.81154C1.73918 4.58798 1.66812 4.35986 1.51237 4.20154L0.834555 3.51247C0.442357 3.11376 0.658775 2.4191 1.20078 2.33696L2.1375 2.195C2.35273 2.16238 2.53879 2.0214 2.63505 1.818L3.05396 0.93275Z"
                        stroke="#EAB270"
                        stroke-width="0.40585"
                        stroke-linejoin="round"
                        class="fill-orange"
                    ></path>
                </svg>

                <svg width="7" height="7" viewBox="0 0 7 7" fill="none" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="none">
                    <path
                        d="M3.05396 0.93275C3.29636 0.420529 3.9967 0.420528 4.2391 0.932749L4.65801 1.818C4.75427 2.0214 4.94033 2.16238 5.15556 2.195L6.09228 2.33696C6.63428 2.4191 6.8507 3.11376 6.45851 3.51247L5.78069 4.20154C5.62494 4.35986 5.55388 4.58798 5.59064 4.81154L5.75065 5.78452C5.84324 6.34751 5.27664 6.77683 4.79186 6.51103L3.95403 6.05165C3.76152 5.94609 3.53154 5.94609 3.33903 6.05165L2.5012 6.51103C2.01642 6.77683 1.44982 6.34751 1.54241 5.78452L1.70242 4.81154C1.73918 4.58798 1.66812 4.35986 1.51237 4.20154L0.834555 3.51247C0.442357 3.11376 0.658775 2.4191 1.20078 2.33696L2.1375 2.195C2.35273 2.16238 2.53879 2.0214 2.63505 1.818L3.05396 0.93275Z"
                        stroke="#EAB270"
                        stroke-width="0.40585"
                        stroke-linejoin="round"
                    ></path>
                </svg>
                </div>
                <p class="text-xs font-bold">Russel766</p>
                <p class="text-xs text-orange">419 followers</p>
            </div>
            <p class="text-sm flex items-center">Jeune artiste souhaitant lancer un skateshop sur Paris, influenceur Instagram</p>
        </div>
        </a>

        <h2 class="w-2/3 font-bold text-lg mb-2">Articles dans la catégorie "Skate"</h2>
        <div class="grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(320px,320px))] justify-around mb-10">
            <a href="achat">
                <Card class="mb-5"
                image="/images/skate-yellow.png"
                :distance="27"
                state="Usé"
                brand="Supreme"
                description="Skate peint lors d’une exposition sur Grenoble, peint à la bombe (peinture sur un modèle de base de Supreme)."
                :price="40"
                title="Skate peint"
                pp="/images/small-painting.jpg"
                :followers="698"
                :star1="true"
                :star2="true"
                :star3="true"
                :star4="true"
                :star5="true"
                :heart="false"
                name="Fabienni"
                :renovation="false"
            /></a>
            <a href="achat">
            <CardDon
            image="/images/skateorange.png"
            :distance="3"
            state="Neuf"
            brand="Santa cruz"
            description="Don de mon skate neuf acheté l’été dernier pendant un voyage en Espagne."
            :price="5"
            title="Skate"
            pp="/images/balland.png"
            :followers="61"
            :star1="true"
            :star2="false"
            :star3="false"
            :star4="false"
            :star5="false"
            :heart="true"
            name="Marie484"/>
            </a>
        </div>

        <h2 class="w-2/3 font-bold text-lg">Dons populaires du jour</h2>
        <h3 class="text-sm font-thin mb-3 text-black">En fonction des articles les plus likés</h3>
        <div class="grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(320px,320px))] justify-around mb-24">
            <a href="achat">
            <Card class="mb-5"
            image="/images/skate-yellow.png"
            :distance="27"
            state="Usé"
            brand="Supreme"
            description="Skate peint lors d’une exposition sur Grenoble, peint à la bombe (peinture sur un modèle de base de Supreme)."
            :price="40"
            title="Skate peint"
            pp="/images/small-painting.jpg"
            :followers="698"
            :star1="true"
            :star2="true"
            :star3="true"
            :star4="true"
            :star5="true"
            :heart="false"
            name="Fabienni"
            :renovation="false"
            />
            </a>
            <a href="achat">
            <CardDon
            image="/images/skateorange.png"
            :distance="3"
            state="Neuf"
            brand="Santa cruz"
            description="Don de mon skate neuf acheté l’été dernier pendant un voyage en Espagne."
            :price="5"
            title="Skate"
            pp="/images/balland.png"
            :followers="61"
            :star1="true"
            :star2="false"
            :star3="false"
            :star4="false"
            :star5="false"
            :heart="true"
            name="Marie484"/>
            </a>
        </div>
    </div>
</template>

<script>
import Card from '../components/Card.vue';
import CardDon from '../components/CardDon.vue';
import SearchBar from "../components/SearchBar.vue"

export default {
    name: "",
    components: {
        Card, CardDon, SearchBar
    },
    created() {
        document.body.style.backgroundColor = "#FFFFFF";
    },
    };
</script>