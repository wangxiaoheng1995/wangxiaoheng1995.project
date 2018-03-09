<template>
  <div class="contact_me">
    <p>住址：{{contact.address}}</p>
    <p>手机：{{contact.number}}</p>
    <p>邮箱：{{contact.email}}</p>
  </div>
</template>
<script type='text/ecmascript-6'>
    export default {
        name: 'contact',
        components: {},
        props:['contact'],
        data() {
            return {
                msg: 'This is vue components.'
            }
        }
    }
</script>
<style scoped lang="stylus" ref="stylesheet/stylus">
.contact_me
  background #fff;
  padding 30px;
  p
    margin-bottom 10px;
  p:last-child
    margin 0;
</style>
