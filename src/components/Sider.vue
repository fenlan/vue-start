<template>
    <div class="nav-side-menu">
        <div class="brand">Brand Logo</div>
        <i class="fa fa-bars fa-2x toggle-btn" data-toggle="collapse" data-target="#menu-content"></i>

        <div class="menu-list">

            <ul id="menu-content" class="menu-content collapse out">
                <li  data-toggle="collapse" data-target="#products" class="collapsed active">
                    <a href="#"><i class="fab fa-studiovinari fa-lg"></i> 核心用户分析 <span class="arrow"></span></a>
                </li>

                <li>
                    <a href="#">
                        <i class="fas fa-tachometer-alt fa-lg"></i> Dashboard
                    </a>
                </li>

                <li data-toggle="collapse" data-target="#service" class="collapsed">
                    <a href="#"><i class="fab fa-fort-awesome-alt fa-lg"></i> Services <span class="arrow"></span></a>
                </li>

                <li data-toggle="collapse" data-target="#new" class="collapsed">
                    <a href="#"><i class="fab fa-pagelines fa-lg"></i> New <span class="arrow"></span></a>
                </li>

                <li>
                    <a href="#">
                        <i class="fas fa-user-tie fa-lg"></i> Profile
                    </a>
                </li>

                <li>
                    <a href="#">
                        <i class="fa fa-users fa-lg"></i> Users
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>
    export default {
    }
</script>

<style scope>
.nav-side-menu {
                overflow: auto;
                font-family: verdana;
                font-size: 14px;
                font-weight: 200;
                background-color: #2e353d;
                position: fixed;
                padding-left: 0px;
                height: 100%;
                width: 14%;
                color: #e1ffff;
            }

            .nav-side-menu .brand {
                background-color: #23282e;
                line-height: 50px;
                display: block;
                text-align: center;
                font-size: 14px;
            }
            .nav-side-menu .toggle-btn {
                display: none;
            }
            .nav-side-menu ul,
            .nav-side-menu li {
                list-style: none;
                padding: 5px;
                margin: 0px;
                line-height: 35px;
                cursor: pointer;
            }
            .nav-side-menu ul .active,
            .nav-side-menu li .active {
                border-left: 3px solid #d19b3d;
                background-color: #4f5b69;
            }
            .nav-side-menu li {
                padding-left: 0px;
                border-left: 3px solid #84a3c6;
                border-bottom: 1px solid #23282e;
            }
            .nav-side-menu li a {
                text-decoration: none;
                color: #e1ffff;
            }
            .nav-side-menu li a i {
                padding-left: 10px;
                width: 20px;
                padding-right: 30px;
            }
            @media (min-width: 767px) {
                .nav-side-menu .menu-list .menu-content {
                    display: block;
                }
            }
</style>
