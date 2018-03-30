# vue-cli 与element-ui学习

## vue-cli的环境搭建

## 安装element-ui

    npm i element-ui -S

## 在main.js中配置使用

    import ElementUI from 'element-ui';
    import 'element-ui/lib/theme-chalk/index.css';

    Vue.use(Element, { size: 'small' });