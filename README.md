搭建步骤：
1. 创建springboot父子项目，修改web项目的application.properties，添加spring.resources.static-locations=classpath:/
2. 在控制台进入web项目D:\user\github\springboot-vue-template\springboot-vue-template-web\src\main\resources下，
执行vue init webpack webapp
3. 修改vue的默认打包路径，打开config目录下的index.js文件，配置build路径
```
// Template for index.html
    index: path.resolve(__dirname, '../../templates/index.html'),

    // Paths
    assetsRoot: path.resolve(__dirname, '../../'),
    assetsSubDirectory: 'static',
    assetsPublicPath: '/',
```
4. 然后执行npm run build，执行完之后启动springboot项目，启动完成通过localhost:8080就可以访问了