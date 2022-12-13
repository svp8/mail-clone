<template>
    <div class="header">
        <div class="header__left">
            <img class="header__left__logo" src="../assets/logo.svg" />
            <img class="filter-logo header__left__text" src="../assets/logo2.svg" />
        </div>
    </div>
</template>
<style lang="scss">
.filter-logo {
    filter: invert(27%) sepia(93%) saturate(5790%) hue-rotate(213deg) brightness(102%) contrast(103%);
}

.header {
    height: 56px;
    padding:12px 16px ;
    &__left {
        height: 32px;
        width: 96px;
        // margin: 12px 16px;
        display: flex;
        gap: 9px;

        // align-items: center;
        &__logo {
            height: 32px;
            width: 32.21641540527344px;
        }

        &__text {
            margin-bottom: 8px;
        }
    }
}
</style>