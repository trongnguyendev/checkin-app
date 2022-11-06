<template>
    <f7-page no-toolbar no-navbar no-swipeback>
        <f7-login-screen-title>Hệ thống chấm công</f7-login-screen-title>
        <f7-login-screen-title>CÔNG TY TNHH LAM VIỆT</f7-login-screen-title>
        
        <f7-block class="text-center">
            <img src="https://cdn.framework7.io/placeholder/people-68x68-1.jpg" width="200" class="m-auto" />
            <p>Trong Nguyen</p>
        </f7-block>
        
        <f7-block>
            <f7-row>
                <f7-col>
                    <f7-button href="/" @click="" round fill raised color="gray" >Thoát</f7-button>
                </f7-col>
                <f7-col>
                    <f7-button href="/dashboard/" @click="" round fill raised >Đăng nhập</f7-button>
                </f7-col>
            </f7-row>
        </f7-block>


        <f7-card>
            <f7-card-content>
                <p class="date">Lưu ý: Bấm "Đăng nhập" để tiếp tục hoặc bấm "Thoát để thoasyt khỏi hệ thống"</p>
                <p>Nếu gặp sự cố đăng nhập vui lòng liên hệ Trong nguyen - 0939.xxx.xxx</p>
            </f7-card-content>
        </f7-card>
    </f7-page>
</template>

<script>
  import { ref, onMounted } from 'vue';
  import { f7, f7ready } from 'framework7-vue';

  export default {
    setup() {    

      return {
      }
    }
  }
</script>