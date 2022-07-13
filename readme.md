基于uni-table修改 增加了最最常用的固定表头的功能
github地址:[https://github.com/1205093639/uni-table-Fixed_header](https://github.com/1205093639/uni-table-Fixed_header)

csdn博客地址:[https://blog.csdn.net/weixin_45391874/article/details/125725971?spm=1001.2014.3001.5502)

实现效果:

![](https://img-blog.csdnimg.cn/e75ba95d0022493c909ca1713cf438ae.gif)

## 1.先找到源码 复制出来单独封装成自己的组件 

![组件源码位置](https://img-blog.csdnimg.cn/b901826229724c5eb24f248fef338f0d.png)
## 2.修改
或者直接下载我的代码

## 3.页面使用

```js
<uni-table border :loading="loading">
                <uni-tr>
                    <uni-th width='80'>序号</uni-th>
                    <uni-th>操作</uni-th>
                    <uni-th>收料单号</uni-th>
                    <uni-th>料号</uni-th>
                    <uni-th>进仓日期</uni-th>
                </uni-tr>
                <uni-tbody height="55vh">
                    <uni-tr v-for='(e,i) in tableData' :key='i'>
                        <uni-td width='80'>{{e.000}}</uni-td>
                        <uni-td>
                            <u-button size="small" @click="toPage(e)" type="primary" text="录入检验结果"></u-button>
                        </uni-td>
                        <uni-td>{{e.111}}</uni-td>
                        <uni-td>{{e.222}}</uni-td>
                        <uni-td>{{e.333}}</uni-td>
                    </uni-tr>
                </uni-tbody>
            </uni-table>
```


附件:[本人已修改的uni_table源码 uni-ui版本1.4.12 提取码:6666](https://pan.baidu.com/s/1AtY6ctMbrrL4HSeSpt2rqg?pwd=6666)
