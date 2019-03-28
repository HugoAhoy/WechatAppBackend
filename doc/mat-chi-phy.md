# 接口文档(数学、语文、物理)

## 数学
<!-- ### 获取集合知识点
> 获取集合知识点，可指定文章的页数，0代表第一页
### URL
/math/set/get
### 接口方法
GET
```json
{
    "openid": "12hsx65cfx",
    "number_every_page": 20,
    "page_offset": 0
}
```
### 返回参数
```json
{
    "code": 0,                                     // 0-成功 其他表示失败，错误码对应具体错误
    "title": "高中数学基础知识点——集合",             // 文章标题
    "content":[
        {
            "id":1,
            "type":,
            "text":,
        },
        {
            "id":2,
            "type":,
            "text":,
        },
        {
            "id":3,
            "type":,
            "text":,
        },
        ...                                       // 根据传入参数，data 列表的长度应该是20
    ]
}
```
### 获取立体几何知识点
> 获取立体几何知识点，可指定文章的页数，0代表第一页
### URL
/math/solidgeometry/get
### 接口方法
GET
```json
{

}
```
### 返回参数
```json
{
    "code": 0,                                     // 0-成功 其他表示失败，错误码对应具体错误
    "title": "高中数学基础知识点——立体几何",         // 文章标题
    "content":[

        ...                                       // 根据传入参数，data 列表的长度应该是20
    ]
}
``` -->


## 语文
###获取高频成语
> 可以指定每页容纳多少组内容，并且是第几页，0代表第一页
### URL
/chinese/idiom/get
### 接口方法
GET
```json
{
    "openid": "12hsx65cfx",
    "number_every_page": 20,
    "page_offset": 0
}
```
### 返回参数
```json
{
    "code": 0,                                     // 0-成功 其他表示失败，错误码对应具体错误
    "title": "高中语文基础知识点——高频成语",         // 文章标题
    "content":[
        {
            "id":1,
            "idiom_1":"按部就班",
            "idiom_2":"循序渐进",
            "explain_1":"指按照一定的条理，遵循一定的程序，通常表达中性或者消极的感情色彩。",
            "explain_2":"指学习、工作等按照一定的步骤逐渐地深人或提高，通常表达中性或者积极的感情色彩。",
            "mistake":"学习并不是一个一蹴而就的过程，而是一个按部就班，逐渐提高的过程。",
            "correction":"句中既然表明了是“逐渐提高”的过程，并不强调按照一定的步骤，而是逐渐深入提高，因此用“循序渐进”要比“按部就班”更为恰当。"
        },
        {
            "id":2,
            "idiom_1":"八面玲珑",
            "idiom_2":"面面俱到",
            "expalin_1":"侧重指为人处事圆滑事故，通常表达消极的感情色彩。",
            "explain_2":"侧重指每个方面都想得很周到，每个细节都予以充分考虑，通常表达中性或积极的感情色彩。",
            "mistake":"他做起事情来八面玲珑，你就放心地把这个任务交给他吧!",
            "correction":"句中“八面玲珑”的感情色彩过于消极，与全句的感情色彩不搭配，因此应该改用“面面俱到”一词。"
        },
        ...                                       // 根据传入参数，data 列表的长度应该是20
    ]
}
```


### 获取词汇拼音
> 可以指定每页容纳多少组内容，并且是第几页，0代表第一页
### URL
/chinese/pinyi/get
### 接口方法
GET
```json
{
    "openid": "12hsx65cfx",
    "number_every_page": 20,
    "page_offset": 0
}
```
### 返回参数
```json
{
    "code": 0,                                     // 0-成功 其他表示失败，错误码对应具体错误
    "title": "高中语文基础知识点——词汇拼音",         // 文章标题
    "content":[
        {
            "id":1,
            "position":2,                           //标注易错读音位置
            "text":"甲壳",                          //词汇文字
            "pinyin":"jiǎ qiào"                     //拼音
        },
        {
            "id":2,
            "position":2,                         //标注易错读音位置
            "text":"藤蔓",                        //词汇文字
            "pinyin":"téng wàn"                   //拼音
        },
        {
            "id":3,
            "position":2,                         //标注易错读音位置
            "text":"不谙水性",                    //词汇文字
            "pinyin":"bù ān shuǐ xìng"           //拼音
        },
        ...                                       // 根据传入参数，data 列表的长度应该是20
    ]
}
```
### 获取易错字型
> 可以指定每页容纳多少组内容，并且是第几页，0代表第一页
### URL
/chinese/mistake_phrase/get
### 接口方法
GET
### 传入参数
>openid: 用户唯一标识ID  
>number_every_page：每页多少单词  
>page_offset：从0开始的页数偏移量，0代表第一页
 
```json
{
    "openid": "12hsx65cfx",
    "number_every_page": 20,
    "page_offset": 0
}
```
### 返回参数
```json
{
    "code": 0,                                     // 0-成功 其他表示失败，错误码对应具体错误
    "title": "高中语文基础知识点——易错字型",         // 文章标题
    "content":[
        {
            "id":1,
            "position":2,                           //标注易错字位置
            "text":"甲壳",                          //词汇文字
            "pinyin":"jiǎ qiào"                     //拼音
        },
        {
            "id":2,
            "position":2,                         //标注易错字位置
            "text":"藤蔓",                        //词汇文字
            "pinyin":"téng wàn"                   //拼音
        },
        {
            "id":3,
            "position":2,                         //标注易错字位置
            "text":"不谙水性",                    //词汇文字
            "pinyin":"bù ān shuǐ xìng"           //拼音
        },
        ...                                       // 根据传入参数，data 列表的长度应该是20
    ]
}
```
### 获取病句
> 获取病句知识点，可以指定每页容纳多少组内容，并且是第几页，0代表第一页
### URL
/chinese/sentence_mis/get
### 接口方法
GET
### 传入参数
>openid: 用户唯一标识ID  
>number_every_page：每页多少单词  
>page_offset：从0开始的页数偏移量，0代表第一页
>type:病句种类,0代表语序不当，1代表搭配不当，2，3，4，5，6，

```json
{
    "openid": "12hsx65cfx",
    "number_every_page": 20,
    "page_offset": 0
}
```
### 返回参数
```json
{
    
}
```

<!-- ### 获取知识归纳
> 空
### URL
/chinese/
### 接口方法
GET
```json
{
    "openid": "12hsx65cfx",
    "number_every_page": 20,
    "page_offset": 0
}
```
### 返回参数
```json
{
    
}
``` -->


## 物理
### 获取
> 空
### URL
/physics/
### 接口方法
GET
```json
{
    "openid": "12hsx65cfx",
    "number_every_page": 20,
    "page_offset": 0
}
```
### 返回参数
```json
{
    
}
```