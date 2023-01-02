# 第一次用VScode写Markdown笔记并上传到github

# Markdown语法笔记
## 一、标题
使用#加空格表示一级标题
使用##加空格表示二级标题
## 二、段落
使用空白行进行分段，并且不要使用缩进

I really like using Markdown.

I think I'll use it to format all of my documents from now on.
## 三、换行
在一行的末尾添加两个或多个空格，然后按回车键,即可创建一个换行  或者直接两个回车
This is the first line.  
And this is the second line.
## 四、强调
### 粗体
在需要加粗的部分前后加两个**或者下划线__  
I just love **bold text**.  
I just love __bold text__.  
### 斜体
在需要加粗的部分前后加一个*或者下划线__  
I just love *bold text*.   
### 粗体和斜体
使用三个*   
I just love ***bold text***. 
## 五、引用  
### 单个段落的块引用 
要创建块引用，请在段落前添加一个 > 符号。  
>Dorothy followed her through many of the beautiful rooms in her castle.  
### 多个段落的块引用  
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.  
## 六、列表
### 有序列表  
要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。   
1. First item
2. Second item   
### 无序列表
要创建无序列表，请在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) ，再紧跟一个空格。缩进一个或多个列表项可创建嵌套列表。   
- First item
* First item
+ First item  
    + First item   
    + Second item
+ First item
### 在列表中嵌套其他元素  
要在保留列表连续性的同时在列表中添加另一种元素  
* This is the first list item.  
* Here's the second list item.  
I need to add another paragraph below the second list item.  
* And here's the third list item.  
### 引用块  
* This is the first list item.  
* Here's the second list item.  
>I need to add another paragraph below the second list item.  
* And here's the third list item.  
### 代码块    
代码块通常采用四个空格或一个制表符缩进。
1.  Open the file.
2.  Find the following code block on line 21:

        * This is the first list item.  
        * Here's the second list item.  

3.  Update the title to match the name of your website.  
### 图片   
![所logo](LG.jpg "西光所logo")    
- 开头一个！   
- 接着一个方括号   
- 后面一个普通括号，里面是图片本地地址或者网络地址及可选标题  
token：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    

## 七、分割线  
单独三个***
***    
## 八、链接  
这是一个链接[我的网站](超链接地址 "超链接title")

## 九、代码高亮
```c
int main(int argv,char *argc[])
{
    char *adc_path="/dev/adc";
    int fd,len;
    char read_buf[512];
    int r;
    memset(read_buf,0,sizeof(read_buf));
    
    if((fd = open(adc_path,O_RDWR|O_NOCTTY|O_NDELAY))<0)
    {

        printf("open adc err \n");
        exit(1);
    }
    
    if((len=read(fd,read_buf,sizeof(read_buf)))<=0)
    {
           printf("adc read err \n");
        exit(1);
    }else
    {
        r= atoi(read_buf);
        r= r*10000/4095;
        printf("adc value is :%d \n",r);
        
    }
    
}
```  










  

