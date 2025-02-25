![TAiOS](./assetes/TAiONS.png)

# TAiONS

> **T**he **A**ria **i**n **O**wari **N**o **S**ekai
>
> 在世界终结时的咏叹调。

一个在线歌词海报生成器是也。

Demo：[https://taions.yuuikic.com/](https://taions.yuuikic.com/)

~~其实是Yuuikic的前端学习和练手项目~~

![Snipaste_2022-01-25_00-46-24](./assetes/home.png)

![example](./assetes/example.png)

## 想要实现的功能

- [x] 搜索歌曲，获取歌词
- [x] 选择歌词 
- [x] 生成海报
- [x] 简单的样式编辑
- [ ] 添加新的API，来自 [Musicmatch](https://developer.musixmatch.com/) 

## 使用步骤

1. 在**搜索框**中输入。
2. 回车，或者点击搜索框上方**图片**搜索。
3. 选中想要生成歌词海报的**歌曲**。
4. 选择想要生成歌词海报的**歌词**。
5. 点击“**箭头**”将选中的歌词添加至海报中。
6. 自定义样式。
7. 手动截图，或者使用“**截图—截图**”来创建一个自动下载的图片文件。
8. 大功告成~

## 注意

1. 搜索歌曲来源平台为网易云音乐。如没有出现想要的歌曲，尝试在搜索时除了填入歌曲名外，额外添加艺术家、专辑名等信息。

2. API请求对IP地址有一定要求，中国大陆的IP可正常返回搜索结果。如果返回的结果与搜索内容完全无关，请优先尝试关闭代理，或者切换到其他区域的IP后再使用。

3. 搜索过程较慢，但一般不会超过10秒。如果过长时间没有反应，请尝试刷新网页。

4. 点击返回的结果获取歌词。点击文字结果会获取原歌词，点击文字右侧专辑图片会获取翻译歌词（如果有翻译歌词可用）

5. 目前可以自定义的样式：背景图片模糊、自定义背景图片、字体、文字颜色、背景色调。

   值得注意的是，由于项目依赖html2canvas的原因，使用“截图—截图”**无法**截取带背景模糊的样式的海报。请通过调节背景透明度以改善文字可读性。

6. GPL V3.0

## 已知问题

1. Firxfox浏览器不支持backdrop-filter这一样式，故宝丽来相纸的背景模糊在Firefox上无法实现（短期内不打算另写一套支持Firefox的样式）

2. 部分屏幕尺寸下显示效果差（比如iPad），只推荐在16：9屏幕的屏幕以及手机设备上使用，其他设备不保证使用效果。

3. 如上文所述，由于项目依赖html2canvas的原因，使用“截图—截图”**无法**截取带背景模糊的样式的海报。并且使用这种方法截图时，图片周围可能会随机地出现1px宽度的白边。

4. You tell me.

## 鸣谢

- 使用[网易云音乐API](https://github.com/Binaryify/NeteaseCloudMusicApi)获取歌曲信息
- 使用[Color Thief](https://github.com/lokesh/color-thief)获取封面主题色
- 使用[html2canvas](https://github.com/niklasvh/html2canvas)获取截图
- 使用[FileSaver.js](https://github.com/eligrey/FileSaver.js/)保存截图图片
- 使用[APlayer](https://aplayer.js.org/#/)作为音乐播放器
- 使用[MetingJS](https://github.com/metowolf/MetingJS)简化播放器使用
- 借鉴了Apple Music的样式（逃）

### 特别鸣谢

   <img src="https://avatars.githubusercontent.com/u/98089914?v=4" alt="" style="height: 100px;border-radius:50%;">    <img src="http://mushengw.cn/wp-content/uploads/2021/11/2AE81886F3B79FA2C99D48DCAF5247EF-e1636376912701.jpg" alt="" style="height: 100px;border-radius:50%;">

一个教会了我一大堆东西

一个没事就跑来和我唠嗑

## 更新日志

**2022/1/28**

1. 新增“宝丽来相纸”样式。
2. 更换生成海报的按钮。

**2022/1/30**

1. 新增字体筑紫A丸，修改默认衬线字体为Noto_Serif
2. 新增调节字体大小功能
3. 大概适配了iOS设备

**2022/2/2/6**

1. 添加了计数器，来自[Moe-counter](https://github.com/journey-ad/Moe-counter)。
