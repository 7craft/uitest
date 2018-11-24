<template>
    <!--this div is create a card-->
    <div class="card">
        <!--this div is create a box as content box-->
        <div class="content">
            <!---in the box got 1 row which is our main content-->
            <div class="row">
                <!--this is the header of the card-->
                <div class="col-xs-5">
                    <slot name="header"></slot>    
                </div>
                <!--this is the main area of Card-->
                <div class="col-xs-7">
                    <slot name ="content"></slot>
                </div>
                <!--this the footer of card-->
                <div class="footer">
                    <hr/>
                    <slot name="footer"></slot>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    export default {
        name: 'box-card'
    }
</script>
<style >

</style>

