### Swiper component for react.

### 运行示例,localhost:3000
```
npm start 
```

### 基本用法
1. 安装并引入react-swiper-lite
```
import Swiper from 'react-swiper-lite'
```
2. 设置相关参数
```
<Swiper
    wrapperClass="wrapperClass"
    itemClass="itemClass"
    itemStyle={{}}
    itemWidth="100%"
    needPadding={false}
    curIdx={1}
    dataList={dataSource}
    prevClass="normal"
    activeClass="active"
    onSlide={onSlide}
    renderItem={renderItem}
    itemClick={itemClick}
    needPagination={true}
    paginationWrapper=""
    paginationPrevClass=""
    paginationActiveClass=""
/>
```

### 参数
- `wrapperClass` String swiper容器样式, 请勿设置transition，会造成卡顿。
- `itemClass` String swiper元素样式
- `itemStyle` Object swiper元素行内样式
- `itemWidth` String 单个swiper元素宽度，范围1%-100%
- `needPadding` Boolean 默认为true,是否需要容器两端留白
- `curIdx` Number 索引，切换swiper元素设置索引即可
- `dataList` Array 数据源，类型为数组
- `prevClass` String 非当前选中swiper样式
- `activeClass` String 当前选中swiper元素样式
- `onSlide` Function 点击或滑动切换到指定索引回调，传入两个参数item,index
- `renderItem` Function 渲染单个swiper子元素布局, 传入两个参数item,index
- `clickTrigger` Boolean 默认为true,点击是否触发切换到改swiper元素
- `itemClick` Function 点击swiper元素回调,传入两个参数item,index。存在该属性则点击不再跳转被点击swiper
- `needPagination` Boolean 默认为false,是否需要分页指示器
- `paginationWrapper` String 指示器父元素样式，可以通过text-align设置指示器位置
- `paginationPrevClass` String 未选中指示器元素样式
- `paginationActiveClass` String 当前选中索引指示器样式
