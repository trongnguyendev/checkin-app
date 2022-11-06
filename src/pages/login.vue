<template>
    <f7-page no-toolbar no-navbar no-swipeback login-screen>
        <f7-login-screen-title>Hệ thống chấm công</f7-login-screen-title>
        <f7-list form>
        <f7-list-input
            label="Mã số nhân viên"
            type="text"
            placeholder="Nhập mã số nhân viên của bạn"
            :value="username"
            @input="username = $event.target.value"
        ></f7-list-input>
        <f7-list-input
            label="Mã xác nhận"
            type="password"
            placeholder="Nhập mã xác nhận của bạn"
            :value="password"
            @input="password = $event.target.value"
        ></f7-list-input>
        </f7-list>
        
        <f7-list>
            <f7-button href="/login-confirm/" @click="signIn" round fill raised >Đăng nhập</f7-button>
        </f7-list>

        <f7-card>
            <f7-card-content>
                <p class="date">Mã xác nhận: mở ứng dụng google authenticator</p>
                <p>Nếu gặp sự cố đăng nhập vui lòng liên hệ Trong nguyen - 0939.xxx.xxx</p>
            </f7-card-content>
        </f7-card>


        <f7-login-screen class="demo-login-screen" :opened="loginScreenOpened" @loginscreen:closed="loginScreenOpened = false">
            <f7-page login-screen>
            <f7-login-screen-title>Framework7</f7-login-screen-title>
            <f7-list form>
                <f7-list-input
                label="Username"
                type="text"
                placeholder="Your username"
                :value="username"
                @input="username = $event.target.value"
                ></f7-list-input>
                <f7-list-input
                label="Password"
                type="password"
                placeholder="Your password"
                :value="password"
                @input="password = $event.target.value"
                ></f7-list-input>
            </f7-list>
            <f7-list>
                <f7-list-button @click="signIn">Sign In</f7-list-button>
                <f7-block-footer>Some text about login information.<br>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</f7-block-footer>
            </f7-list>
            </f7-page>
        </f7-login-screen>
    </f7-page>
</template>

<script>
  import { ref, onMounted } from 'vue';
  import { f7, f7ready } from 'framework7-vue';

  export default {
    setup() {

      // Login screen data
      const username = ref('');
      const password = ref('');

      const signIn = () => {
        
        f7.dialog.alert('Username: ' + username.value + '<br>Password: ' + password.value, () => {
          f7.loginScreen.close();
        });
      } 
      onMounted(() => {
        f7ready(() => {


          // Call F7 APIs here
        });
      });

      return {
        username,
        password,
        signIn
      }
    }
  }
</script>