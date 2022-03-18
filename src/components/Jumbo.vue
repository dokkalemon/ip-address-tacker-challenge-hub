<template>
    <section class="jumbo full-width">
        <div class="back">
            <img src="@/assets/pattern-bg.png" alt="">
        </div>

        <div class="main-content container px-20">
            <h1>IP Address Tracker</h1>
            <div class="search">
                <input type="text" placeholder="Search for any IP address or domain">
                <button><img src="@/assets/icon-arrow.svg" alt=""></button>
            </div>
        </div>


    </section>
</template>

<script>
export default {
    name: 'JumboComponent'
}
</script>

<style lang="scss" scoped>
@import '@/scss/variables';

.jumbo {
    height: 35vh;
    position: relative;
    .back {
        height: 100%;
        width: 100%;
        position: absolute;
        top: 0;
        left: 0;
        img {
            height: 100%;
            width: 100%;
            object-fit: cover;
        }
    }
    .main-content {
        position: relative;
        z-index: 5;
        padding-top: 50px;
        display: flex;
        flex-direction: column;
        align-items: center;
        h1 {
            font-weight: 500;
            color: white;
            text-align: center;
            font-size: 35px;
        }
        .search {
            padding-top: 30px;
            input {
                height: 60px;
                width: 480px;
                padding: 0 20px;
                font-size: 18px;
                border-radius: 20px 0 0 20px;
                border: none;
                color: $very-dark-gray;
                outline: none;
            }
            button {
                background-color: #000000;
                height: 60px;
                width: 60px;
                border: none;
                border-radius: 0 20px 20px 0;
                cursor: pointer;
                &:hover {
                    background-color: $very-dark-gray;
                }
            }
        }
    }
}




</style>