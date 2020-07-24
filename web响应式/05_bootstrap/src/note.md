### 布局系统
栅格布局，bootstrap4.x 以移动端优先 576/768/997/1200
container：左右padding:15px
container-fuild:没有内边距

### 栅格等级
.col : 小于超小屏幕 <576px , 不管多小都不会换行
.col-sm : 大于小屏幕 >=576px , 
.col-md : >=768px
.col-lg : >=992px
.col-xl : >=1140px

意思就是屏幕宽度符合我们定义的某一区间等级中，就按这个等级设定值排版

### 设置显示和隐藏
可以控制元素在不同设备上的显/隐
.d-[sm|md|lg|xl] : 隐藏  这个语法和 bs3.x中的 hidden-[sm|md|lg|xl] 效果一样

### 对齐和排序
对齐：原理等于flex
.align-items-[start|center|end] : 作用于父元素：垂直方向的子元素排列方式
.justify-content-[start|center|end|around|between] : 水平方向子元素的排列方式
.align-self-[start|center|end] : 子元素自身的排列方式，可以一个个对子元素排列
.order-[1~12] : 指定子元素的顺序，1最先，然后其次，或者 order-[first|last]
.offset-N 或 .offset-*-N 设置偏移量:N为栅格列数 (1-12)

### 内容排版
1. 标题类
h1~h6:重写过，可以直接在元素中: class="h1"
.display-[1|2|3|4] : 1最醒目，然后其次

2. 文本类
.lead : 强调文本
来自html5的文本标签 : strong|mark|del|s|u|ins|samll|em

3. 列表类
.list-unstyled ： 初始化列表样式

4. 图文样式
1) 给图片添加一个 .img-fluid 样式（自适应）或者设置 max-width:100%;height:auto;
2) 图片缩略图,img-thumbnail
3) float-[left|right] : 设置浮动
4) .d-block 设为区块，然后 .mx-auto(margin 左右 auto 实现居中)
5) 图片本身是内联块属性，直接父层 .text-center 也可以实现居中
6) <picture> html5的响应式图片标签
7) figgure figcaption 图文组合显示

### 颜色和边框
1. 颜色:选择比较有限
.text-* 指定文本颜色
.bg-*   指定背景颜色

2. 边框样式
.border-[left|right|bottom|top] : 
.border-0 ： 消除边框  border-[left|right|bottom|top]-0 : 消除某一边
.rounded 和 .rounded-[] 实现各种方位圆角

### 工具类

