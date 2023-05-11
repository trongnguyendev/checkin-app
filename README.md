# My App

## Framework7 CLI Options

#api/modules/test.api.js
```
import axios from "axios"
const BASE_URL = 'http://localhost:8000/api';

const api = () => {
    return {
        async getTest() {
            return await axios.get(BASE_URL + "/test");
        },
    }
}
```
#api/index.js
```
import test from "./modules/test.api"

export default {
    test
}

export default api;
```

#store/index.js
```
import { createStore } from "vuex"
import api from '../api'
const store = createStore({
  state: {},
  getters: {},
  mutations: {},
  actions: {
    async getTest({ commit }) {
      let res = await api.test().getTest();
      return res;
    }
  }
})

export default store;
```
#helper
```
export default {
  randomStr(str) {
    return str;
  }
}
```

#Responsive
```
Điện thoại di động (thường dưới 768px)
Máy tính bảng (từ 768px đến 1024px)
Màn hình máy tính và laptop (từ 1024px đến 1440px)
Màn hình lớn (từ 1440px trở lên)
```

Framework7 app created with following options:

```
{
  "cwd": "D:\\dev\\project1",
  "type": [
    "web"
  ],
  "name": "My App",
  "framework": "vue",
  "template": "single-view",
  "cssPreProcessor": "scss",
  "bundler": "vite",
  "theming": {
    "customColor": false,
    "color": "#007aff",
    "darkTheme": false,
    "iconFonts": true,
    "fillBars": false
  },
  "customBuild": false
}
```

## Install Dependencies

First of all we need to install dependencies, run in terminal
```
npm install
```

## NPM Scripts

* 🔥 `start` - run development server
* 🔧 `dev` - run development server
* 🔧 `build` - build web app for production

## Vite

There is a [Vite](https://vitejs.dev) bundler setup. It compiles and bundles all "front-end" resources. You should work only with files located in `/src` folder. Vite config located in `vite.config.js`.
## Assets

Assets (icons, splash screens) source images located in `assets-src` folder. To generate your own icons and splash screen images, you will need to replace all assets in this directory with your own images (pay attention to image size and format), and run the following command in the project directory:

```
framework7 assets
```

Or launch UI where you will be able to change icons and splash screens:

```
framework7 assets --ui
```



## Documentation & Resources

* [Framework7 Core Documentation](https://framework7.io/docs/)
* [Framework7 Vue Documentation](https://framework7.io/vue/)


* [Framework7 Icons Reference](https://framework7.io/icons/)
* [Community Forum](https://forum.framework7.io)

## Support Framework7

Love Framework7? Support project by donating or pledging on:
- Patreon: https://patreon.com/framework7
- OpenCollective: https://opencollective.com/framework7
