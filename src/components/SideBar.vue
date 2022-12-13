<template>
    <div class="sidebar">
        <button class="sidebar__button text-700">Написать письмо</button>
        <ul class="sidebar__folders">
            <li v-for="folder in folders" :key="folder.id" class="sidebar__folders__item">
                <img class="sidebar__folders__item__icon" :src="require(`@/assets/${folder.icon}`)" />
                <span class="text-400 sidebar__folders__item__text">{{ folder.name }}</span>
            </li>
        </ul>
        <hr class="sidebar__border" />
        <div class="sidebar__folders__item">
            <img class="sidebar__folders__item__icon-new" src="../assets/Plus.svg"/>
            <span class="text-500 sidebar__folders__item__text">Новая папка</span>
        </div>
    </div>
</template>
<script>
import { folders } from "@/utils/folders.js"
export default {
    setup() {
        // const folders = [{ id: 1, icon: "", name: "lolz" }]
        return { folders }
    }
}
</script>
<style lang="scss">
.sidebar {
    padding-left: 16px;
    padding-right: 16px;

    &__button {
        background-color: white;
        height: 36px;
        width: 200px;
        border-radius: 8px;
        border: 1px solid #00103D1F;
        margin-bottom: 12px;
    }

    &__folders {
        &__item {
            position: relative;
            cursor: pointer;
            border-radius: 8px;
            height: 36px;
            padding: 8px 12px;
            gap: 10px;
            display: flex;
            flex-direction: row;
            align-items: center;
            &__icon-new{
                filter: invert(59%) sepia(4%) saturate(481%) hue-rotate(187deg) brightness(92%) contrast(82%);
            }
            &__text {
                position: absolute;
                left: 40px
            }

            &:hover {
                background-color: rgba(0, 16, 61, 0.04);
            }
        }
    }

    &__border {
        background: rgba(0, 16, 61, 0.12);
        margin-bottom: 8px;
        margin-top: 8px;
    }
}
</style>