<template>
    <div class="sidebar">
        <nav>
            <ul class="sidebar-nav">
                <a href="">
                    <li>
                        <span class="icon-container"><i class="material-icons">dashboard</i></span>
                        <span class="nav-item">Dashboard</span> 
                    </li>
                </a>
                <a href="">
                <li>
                    <i class="material-icons">forward</i>
                    <span class="nav-item">Tickets</span>
                </li>
                </a>
                <a href="">
                    <li><i class="material-icons">exit_to_app</i><span class="nav-item">Logout</span></li>
                </a>
            </ul>
        </nav>
    </div>
    
</template>


<script>
export default {
    name: 'sidebar'
    
}
</script>

<style lang="scss">

@import '../global.scss';

    .sidebar{
        background: #313131;
        display: flex;
        min-width: 200px;
        z-index: 8899;
        nav{
            width: 100%;
        }
    }



    ul.sidebar-nav{
        padding: 2em 0;


                a{
                    text-decoration: none;
                    color: $color-grey-light;
                    font-family: $paragraph;
                    @include size(14px);

                    li{
                padding: 7px 0 18px 20px;
                border-bottom: 1px solid $color-grey-dark;
                
                    span.nav-item {
                        padding-left: 10px;
                    }
                }
            }   

    }


i.material-icons {
    position: relative;
    top: 7px;
}


 
</style>

