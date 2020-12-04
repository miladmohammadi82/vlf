<template>
    <header class="mt-4 header-section">
        <div class="row ml-auto justify-content-md-between justify-content-sm-between">
            <ul class="d-flex">
                <li>
                    <div class="menu-btn" :class="{ open:menuOpen }" @click="menuOpenshow">
                        <i class="fas fa-bars fa-2x"></i>
                    </div>
                </li>
                <li>      
                    <div class="menu-btn-user" :class="{ openUser:menuOpenUser }" @click="menuOpenUsershow">
                        <i class="fas fa-user fa-2x"></i>
                    </div>
                </li>
            </ul>
            

            <div class="mr-5">
                <h2>LOGO</h2>
            </div>
            
            <nav class="d-flex nav main-menu" :class="{ show:mobileMenu }">
                
                
            
                <li class="nav-link">صفحه اصلی</li>
                <li class="nav-link">فرانت اند <i class="fas fa-angle-down"></i>
                    <div class="dropdown">
                        <ul>
                            <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                        </ul>
                    </div>
                </li>
                <li class="nav-link">بک اند <i class="fas fa-angle-down"></i>
                    <div class="dropdown">
                            <ul>
                                <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                                <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                                <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                            </ul>
                        </div>
                    </li>
                <li class="nav-link">زبان ها <i class="fas fa-angle-down"></i>
                    <div class="dropdown">
                        <ul>
                            <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                        </ul>
                    </div>
                </li>
                <li class="nav-link">رابط کاربری <i class="fas fa-angle-down"></i>
                    <div class="dropdown">
                        <ul>
                            <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                        </ul>
                    </div>
                </li>
                <li class="nav-link">گرافیک <i class="fas fa-angle-down"></i>
                    <div class="dropdown">
                        <ul>
                            <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                        </ul>
                    </div>
                </li>
                <li class="nav-link">CMS ها <i class="fas fa-angle-down"></i>
                    <div class="dropdown">
                        <ul>
                            <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                            <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                        </ul>
                    </div>
                </li>
            </nav>

            <!-- Menu Mobile -->

            <div class="mobile-menu" :class="{ showMenu:mobileMenu }">
                <div class="head-menu-mobile">
                    <div class="head-menu-mobile">
                        <div class="clise-nav" @click="menuOpenshow">
                            <i class="far fa-times fa-2x"></i>
                        </div>
                    </div>
                    <form action="" class="searchBox"> 
                        <div class="input-group input-group-lg">
                            <input type="text" placeholder="ترجمه ...">
                            <button><i class="far fa-search" style="font-size: 15px;"></i></button>
                        </div>
                    </form>
                </div>

                <nav class="menu-main">
                    <ul>
                        <li><a href="#">صفحه اصلی</a></li>
                        <li class="nav-link"><a href="#">فرانت اند</a>
                        <i class="fas fa-angle-down"></i>
                        <div class="dropdown">
                            <ul>
                                <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                                <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                                <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                            </ul>
                        </div>
                        </li>
                        <li class="nav-link"><a href="#">بک اند</a>
                        <i class="fas fa-angle-down"></i>
                            <div class="dropdown">
                                    <ul>
                                        <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                                        <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                                        <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                                    </ul>
                                </div>
                            </li>
                        <li class="nav-link"><a href="#">زبان ها</a>
                        <i class="fas fa-angle-down"></i>
                            <div class="dropdown">
                                <ul>
                                    <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                                    <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                                    <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                                </ul>
                            </div>
                        </li>
                        <li class="nav-link"><a href="#">رابط کاربری</a>
                        <i class="fas fa-angle-down"></i>
                            <div class="dropdown">
                                <ul>
                                    <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                                    <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                                    <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                                </ul>
                            </div>
                        </li>
                        <li class="nav-link"><a href="#">گرافیک</a>
                        <i class="fas fa-angle-down"></i>
                            <div class="dropdown">
                                <ul>
                                    <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                                    <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                                    <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                                </ul>
                            </div>
                        </li>
                        <li class="nav-link"><a href="#">CMS ها</a>
                        <i class="fas fa-angle-down"></i>
                            <div class="dropdown">
                                <ul>
                                    <li class="dropdown-link"><a href="#">آیتم 1</a></li>
                                    <li class="dropdown-link"><a href="#">آیتم 2</a></li>
                                    <li class="dropdown-link"><a href="#">آیتم 3</a></li>
                                </ul>
                            </div>
                        </li>
                    </ul>
                </nav>


            </div>

            <!-- Menu Mobile -->

            <div :class="{ overlay:mobileMenu }" @click="menuOpenshow"></div>

            <div class="logr d-flex align-items-lg-center ml-4">
                <btn-prime-flat class="fas fa-search search-btn ml-2"></btn-prime-flat>
                <btn-prime-flat style="border-bottom: 2px solid #023e8a;">ثبت نام</btn-prime-flat>
                <btn-sccss-flat style="border-bottom: 2px solid #0ead69;" class="mr-3">ورود</btn-sccss-flat>
            </div>


            <div class="menu-user" :class="{ showUser:menuOpenBoxUser }">
                <div class="head-menu-user">
                   
                        
                    
                    <a href="#" @click="menuOpenUsershow" class="clise-nav2"><i class="far fa-times fa-2x"></i></a>

                    <img src="../../assets/image-profile.jpg" class="text-center best-teacher-avatar"  alt="">
                    <h4>میلاد محمدی</h4>
                </div>
                
                
                <ul>
                    <li class="user-link"><a href="#"><i class="fas fa-user"></i>&nbsp;&nbsp;حساب کاربری</a></li>
                    <li class="user-link"><a href="#"><i class="fas fa-user"></i>&nbsp;&nbsp;حساب کاربری</a></li>
                    <li class="user-link"><a href="#"><i class="fas fa-user"></i>&nbsp;&nbsp;حساب کاربری</a></li>
                    <li class="user-link"><a href="#"><i class="fas fa-user"></i>&nbsp;&nbsp;حساب کاربری</a></li>
                    <li class="user-link"><a href="#"><i class="fas fa-user"></i>&nbsp;&nbsp;حساب کاربری</a></li>
                </ul>
            </div>

            <div :class="{ overlay:menuOpenBoxUser }" @click="menuOpenUsershow"></div>

        </div>

        <div class="row container-fluid header-2">
            <div class="col-lg-6 d-flex flex-column justify-content-center head-center">
                <h1>با ویرولرن</h1>
                <h2 class="mt-3">لحظه ای از تکنولوژی عقب نمانید !</h2>
                <p class="mt-3 head-p">آموزش آنلاین توسط بهترین اساتید برای ساخت آینده کاری شما و تضمین یادگیری شما در ویرولرن</p>
                <div class="buttons mt-5">
                    <btn-warn-out>از دوره های ما دیدن کنید</btn-warn-out>
                    <btn-prime-out>از فروشگاه ما دیدن کنید</btn-prime-out>
                </div>
            </div>

            <div class="col-lg-6 online-course"></div>
        </div>
    </header>
</template>

<script>
    import btnPrimeFlat from "../buttons/primary/flat";
    import btnPrimeOut from "../buttons/primary/outline";
    import btnWarnOut from "../buttons/warning/outline";
    import btnSccssFlat from "../buttons/success/flat";
    export default {
        name: "Header",
        data(){
            return{
                menuOpen: false,
                mobileMenu: false,
                menuOpenUser: false,
                menuOpenBoxUser:false,
                showOpenIconMobile:false,
            }
        },

        methods: {
            menuOpenshow(){
                if(!this.menuOpen){
                    this.menuOpen = true
                }else{
                    this.menuOpen = false
                }

                if(!this.mobileMenu){
                    this.mobileMenu = true
                }else{
                    this.mobileMenu = false
                }

                if(this.mobileMenu && this.menuOpenUser && this.menuOpenBoxUser){
                    this.menuOpenUser = false
                    this.menuOpenBoxUser = false
                }
            },

            menuOpenUsershow(){
                if(!this.menuOpenUser){
                    this.menuOpenUser = true
                }else{
                    this.menuOpenUser = false
                }

                if(!this.menuOpenBoxUser){
                    this.menuOpenBoxUser = true
                }else{
                    this.menuOpenBoxUser = false
                }

                if(this.menuOpenBoxUser && this.menuOpen && this.mobileMenu){
                    this.menuOpen = false
                    this.mobileMenu = false
                }
            },

            openIconMibile(){
                if(!this.showOpenIconMobile){
                    this.showOpenIconMobile = true
                }
            }

        },

        components: {
            btnPrimeFlat,
            btnPrimeOut,
            btnWarnOut,
            btnSccssFlat,
        },

        
    };
</script>
