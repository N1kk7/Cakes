<template>
    <div class="footerBg">
        <div class="footer">
            <h1>this is footer</h1>


        </div>

    </div>
</template>

<script>


</script>

<style lang="scss">
    .footerBg{
        background-color: antiquewhite;
        .footer{
        background-color: rgb(48, 30, 6);
        height: -webkit-fill-available;
        --mask:
            radial-gradient(56.60px at 50% 78.00px,#000 99%,#0000 101%) calc(50% - 60px) 0/120px 100%,
            radial-gradient(56.60px at 50% -48px,#0000 99%,#000 101%) 50% 30px/120px 100% repeat-x;
        -webkit-mask: var(--mask);
                mask: var(--mask);
       
        min-height: 30vh;
    }

    }
    


</style>