<template>
    <footer id="footer-3" class="pt-100 footer ft-3-ntr">
        <div class="container">
            <!-- FOOTER CONTENT -->
            <div class="row">
                <!-- FOOTER LOGO -->
                <div class="col-xl-3">
                    <div class="footer-info">
                        <img class="footer-logo" src="/assets/images/EISPEDN-EN-Logo.png" alt="footer-logo" />
                    </div>
                </div>
                <!-- FOOTER LINKS -->
                <div class="flex flex-col md:flex-row justify-between">
                    <div class="footer-links fl-1">
                        <!-- Title -->
                        <NuxtLink to="/"  class="s-17 px-4 py-2 rounded text-white cursor-pointer bg-blue-500 hover:bg-blue-300 " @click="scrollToTop()">Home</NuxtLink>
                        <!-- Links -->
                       
                    </div>
                    <div class="footer-links fl-1">
                        <!-- Title -->
                        <NuxtLink to="" class="s-17 px-4 py-2 rounded text-white cursor-pointer bg-blue-500 hover:bg-blue-300 ">Activities</NuxtLink>
                        <!-- Links -->
                       
                    </div>
                    <div class="footer-links fl-1">
                        <!-- Title -->
                        <NuxtLink to="" class="s-17 px-4 py-2 rounded text-white cursor-pointer bg-blue-500 hover:bg-blue-300 ">Gallery</NuxtLink>
                        <!-- Links -->
                       
                    </div>
                    <div class="footer-links fl-1">
                        <!-- Title -->
                        <NuxtLink to="" class="s-17 px-4 py-2 rounded text-white cursor-pointer bg-blue-500 hover:bg-blue-300 ">Patient Materials</NuxtLink>
                        <!-- Links -->
                       
                    </div>
                    <div class="footer-links fl-1">
                        <!-- Title -->
                        <NuxtLink to="" class="s-17 px-4 py-2 rounded text-white cursor-pointer bg-blue-500 hover:bg-blue-300 ">About Us</NuxtLink>
                        <!-- Links -->
                       
                    </div>
                    <div class="footer-links fl-1">
                        <!-- Title -->
                        <NuxtLink to="" class="s-17 px-4 py-2 rounded text-white cursor-pointer bg-blue-500 hover:bg-blue-300 ">Contact Us</NuxtLink>
                        <!-- Links -->
                       
                    </div>
                    
                </div>
                   
                <!-- END FOOTER LINKS -->
                <!-- FOOTER NEWSLETTER FORM -->
                <div class="col-sm-10 col-md-8 col-lg-4 col-xl-3">
                    <div class="footer-form">
                        <!-- Title -->
                        <h6 class="s-17 w-700">Follow the Best</h6>
                        <!-- Newsletter Form Input -->
                        <form class="newsletter-form">
                            <div class="input-group r-06">
                                <input type="email" class="form-control" placeholder="Email Address" required id="s-email" />
                                <span class="input-group-btn ico-15">
                                    <button type="submit" class="btn color--theme">
                                        <span class="flaticon-right-arrow-1"></span>
                                    </button>
                                </span>
                            </div>
                            <!-- Newsletter Form Notification -->
                            <label for="s-email" class="form-notification"></label>
                        </form>
                    </div>
                </div>
                <!-- END FOOTER NEWSLETTER FORM -->
            </div>
            <!-- END FOOTER CONTENT -->
            <hr />
            <!-- FOOTER DIVIDER LINE -->
            <!-- BOTTOM FOOTER -->
            <div class="bottom-footer">
                <div class="row row-cols-1 row-cols-md-2 d-flex align-items-center">
                    <!-- FOOTER COPYRIGHT -->
                    <div class="col">
                        <div >
                            <span class="p-sm flex items-center justify-center mx-auto text-center gap-1">&copy; 2024 <nuxt-link class="cursor-pointer" target="_blank" to="https://www.skylink-eg.com/">
                                <img class="rounded w-40" src="https://www.skylink-eg.com/images/logo.png" alt=""></nuxt-link>  <span>All Rights Reserved</span> </span>
                        </div>
                    </div>
                    <!-- FOOTER SOCIALS -->
                    <div class="col">
                        <ul class="bottom-footer-socials ico-20 text-end">
                            <li>
                                <a href="#"><span class="flaticon-facebook"></span></a>
                            </li>
                            <li>
                                <a href="#"><span class="flaticon-twitter"></span></a>
                            </li>
                            <li>
                                <a href="#"><span class="flaticon-instagram"></span></a>
                            </li>
                            <li>
                                <a href="#"><span class="flaticon-youtube"></span></a>
                            </li>
                        </ul>
                    </div>
                </div>
                <!-- End row -->
            </div>
            <!-- END BOTTOM FOOTER -->
        </div>
        <!-- End container -->
        <FooterGoToTop />
    </footer>
</template>
<script setup>
const scrollToTop = () => {
  window.scrollTo({ top: 0, behavior: 'smooth' })
}
</script>
