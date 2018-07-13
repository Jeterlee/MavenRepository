## MavenRepository
- **项目说明**：搭建的私人`Maven`仓库，存放个人项目的依赖包，使用Github统一管理。
- **原理说明**：Github使用了`raw.githubusercontent.com`这个域名用于raw文件下载。
- **使用说明**：使用自定义仓库的地址（见下面），在线式或离线式使用配置文件。


## 如何添加依赖
step1、添加自定义仓库的地址
```gradle
repositories {  
    jcenter()
    maven {
        // 自定义仓库的地址
        url "https://raw.githubusercontent.com/Jeterlee/MavenRepository/master"
    }
}
```

step2、dependencies下增加需要添加的依赖
```gradle
dependencies{  
    implementation ...  
} 
```


## 参考资料
- [**Android Studio 将github作为远程maven仓库（推荐阅读）**](http://blog.csdn.net/leilba/article/details/49367271)
- [AndroidStudio使用进阶二：搭建自己的maven私服，并使用Gradle统一依赖管理](http://blog.csdn.net/jf_1994/article/details/51228560)
- [基于Github搭建Maven仓库的方法](http://www.jianshu.com/p/3111bcf96cdf)
- [利用github搭建个人maven仓库](http://blog.csdn.net/hengyunabc/article/details/47308913)


## License
```
Copyright (c) 2017 - 2018, The Jeterlee authors 

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```
