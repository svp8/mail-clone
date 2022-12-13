<template>
    <div class="main">
        <SideBar class="main__sidebar"></SideBar>
        <LetterList></LetterList>
    </div>
</template>
<script>
import SideBar from './SideBar.vue'
import LetterList from './LetterList.vue';
export default {
  components: {
    SideBar,
    LetterList
  }
}
</script>
<style lang="scss">
.main{
    background-color:#F6F7F8 ;
    height: max-content;
    flex: 1;
    display: flex;
    padding-top: 12px;
    &__sidebar{
        margin-left:16px
    }
    &__content{
        flex:1
    }
}
</style>