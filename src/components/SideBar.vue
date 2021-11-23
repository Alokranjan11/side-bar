<template>
    <div :class="[show ? 'sideBarafterClose' : 'sideBarBeforeClose', 'sidebarmain']">
        <div class="sideBar">
            <i v-if="!show" @click="showSideBar()" class="fas fa-bars font-large"></i>
            <div v-else>
              <i  @click="showSideBar()" class="fas close-icon fa-arrow-circle-left font-large"></i>
            </div>
            <span class="font-large">Menu</span>
        </div>
        <div class="sideBar">
            <i class="fas fa-columns font-large"></i>
            <span>Dashboard</span>
        </div>
        <div class="sideBar">
            <i class="fas fa-user font-large"></i>
            <span>User</span>
        </div>
        <div class="sideBar">
            <i class="fas fa-car font-large"></i>
            <span>Messages</span>
        </div>
        <div class="sideBar">
            <i class="fas fa-folder-minus font-large"></i>
            <span>File Manager</span>
        </div>
        <div class="sideBar">
            <i class="fas fa-save font-large"></i>
            <span>Saved</span>
        </div>
        <div class="sideBar">
            <i class="fas fa-cog font-large"></i>
            <span>Setting</span>
        </div>
        <div class="sideBar">
            <i class="fas fa-hashtag font-large"></i>
            <span>Socail Media</span>
        </div>
        <div class="sideBar">
            <i class="fas fa-user-circle font-large"></i>
            <span>Alok Ranjan</span>
            <!-- <span>Software Developer</span> -->
        </div>
    </div>
</template>

<script>
export default {
    name: "SideBar",
    data() {
        return {
            show: false,
        };
    },
    methods: {
        showSideBar() {
            this.show = !this.show;
        },
    },
};
</script>

<style scoped>
.sidebarmain {
    background-color: rgb(10, 10, 10, 0.9);
    color: #ffff;
    width: 300px;
    height: 100vh;
    border-radius: 0px 0px 20px 0px;
    overflow: hidden;
    position: fixed;
    top: 80px;
    left: 0px;
}
/* .sidebarmain:hover{
    overflow:visible;
} */
.sideBar {
    padding: 20px;
    margin: 10px;
    display: flex;
    height: 25px;
    cursor: pointer;
}
.sideBar:hover {
    color: rgb(10, 10, 10);
    /* color:var(--red-500); */
    /* color: rgb(33, 33, 185); */
    background-color: #ffff;
    border-radius: 0px 20px 0px 20px;
}
.sideBar span {
    margin-left: 30px;
    font-size: 20px;
    font-weight: 700;
}
.sideBarAfterClose {
    width: 350px;
}
.sideBarBeforeClose {
    width: 78px;
}
.close-icon {
    position: absolute;
    right: 20px;
}
</style>
