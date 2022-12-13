<template>
    <div class="list">
        <ul class="list__letters">
            <li class="list__letters__item">
                <span>.</span>
                <img class="list__letters__item__img" />
                <h1 class="list__letters__item__name">Имя 123</h1>
                <img class="list__letters__item__fav" />
                <div class="list__letters__item__">
                    <div>
                        <h1>Тема</h1>
                        <h1>Сообщение</h1>
                    </div>

                    <div>
                        <div>

                        </div>
                        <time>13:12</time>
                    </div>
                </div>


            </li>
        </ul>
    </div>
</template>
<style lang="scss">
.list {
    background: #FFFFFF;
    border-radius: 12px;
    flex: 1;

    &__letters {
        display: flex;
        flex-direction: column;

        &__item {
            display: flex;
            background: #FFFFFF;
            border-radius: 12px;

            &__img {
                height: 32px;
                width: 32px;

            }
        }
    }
}
</style>