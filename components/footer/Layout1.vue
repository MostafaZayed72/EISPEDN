<template>
    <footer id="footer-3" class="pt-100 footer ft-3-ntr">
        <div class="container">
            <!-- FOOTER CONTENT -->
            <div class="row">
                <!-- FOOTER LOGO -->
                
                <!-- FOOTER LINKS -->
                
                   
                <!-- END FOOTER LINKS -->
                <!-- FOOTER NEWSLETTER FORM -->
               
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
