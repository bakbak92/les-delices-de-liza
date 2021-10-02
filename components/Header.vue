<template>
    <header>
        <nav>
            <nuxt-link to="/">
                <span class="logo">Les <span>délices</span> de liza</span>
            </nuxt-link>
            <ul>
                <li>
                    <nuxt-link to="/menu">
                    Menu
                    </nuxt-link>
                </li>
            </ul>
        </nav>
    </header>
</template>
<style lang="scss">
@import "../assets/css/colors.scss";

header{
    nav{
        padding: 20px;
        display: flex;
        justify-content: space-between;
        color: $brown;
        a{
            text-decoration: none;
            color: $brown;
        }
        .logo{
            font-size: 20px;
            font-weight: 600;
        }
        ul{
            list-style: none;
            display: flex;
            margin: 0;
            li{
                margin-left: 20px;
                a{
                    text-transform: uppercase;
                    cursor: pointer;
                    &:hover{
                        border-bottom: 2px solid $gold;
                    }
                }
            }
        }
    }
}
</style>