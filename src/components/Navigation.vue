<template>
  <div>
    <header :class="{'scrolled-nav' :scrolledNav}">
        <nav>
            <div class="branding">

            </div>
            <ul v-show="!mobile" class="navigation">
                <li><router-link class="link" :to="{ name: 'Home' }">Home</router-link></li>
                <li><router-link class="link" :to="{ name: '' }">Data Barang</router-link></li>
                <li><router-link class="link" :to="{ name: '' }">Peminjaman</router-link></li>
                <li><router-link class="link" :to="{ name: '' }">Riwayat</router-link></li>
            </ul>
            <div class="icon">
                <i @click="toggleMobileNav" v-show="mobile" class="far fa-bars" :class="{'icon-active': mobileNav}"></i>
            </div>
            <transition name="mobile-nav">
                <ul v-show="!mobile" class="navigation">
                    <li><router-link class="link" :to="{ name: 'Home' }">Home</router-link></li>
                    <li><router-link class="link" :to="{ name: '' }">Data Barang</router-link></li>
                    <li><router-link class="link" :to="{ name: '' }">Peminjaman</router-link></li>
                    <li><router-link class="link" :to="{ name: '' }">Riwayat</router-link></li>
                </ul>
            </transition>
        </nav>
    </header>
  </div>
</template>

<script>
export default {
    name: "navigation",
    data() {
        return {
            scrolledNav: null,
            mobile: true,
            mobileNav: true,
            windowWidt: null,
        }
    }
};
</script>


<style lang="scss" scoped>
header {
    background-color: rgb(0, 0, 0, 0.8);
    z-index: 90;
    width: fixed;
    transition: 0.5s ease all;
    color: #ffff;

    nav {
        display: flex;
        flex-direction: row;
        padding: 12px 0;
        transition: 0.5 ease all;
        width: 90%;
        margin: 0 auto;
        @media (min-width: 1140px) {
            max-width: 1140px;
        }

        ul {
            .link {
                font-weight: 500;
                color: #ffff;
                list-style: none;
                text-decoration: none;
            }
        }

        li {
            text-decoration: uppercase;
            padding: 16px;
            margin-left: 16px;
        }

        .link {
            font-size: 14px;
            transition: 0.5s ease all;
            padding-bottom: 4px;
            border-bottom: 1px solid transparent;

            &:hover {
                color: #00afea;
                border-color: #00afea;
            }
        }

        .branding {
            display: flex;
            align-items: center;
            img {
                width: 50px;
                transition: 0.5s ease all;
            }
        }

        .navigation {
            display: flex;
            align-items: center;
            flex: 1;
            justify-content: flex-end ;
        }

        .icon {
            display: flex;
            align-items: center;
            position: absolute;
            top: 0;
            right: 24px;
            height: 100%;

            i {
                cursor: pointer;
                font-size: 24px;
                transition: 0.8s ease all;
            }
        }
        .icon-active {
            transform: rotate(180deg);
        }
    }
}
</style>