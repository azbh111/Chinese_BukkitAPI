#Chinese_BukkitAPI
__翻译前必须阅读此页！！！__
##====****项目说明****====
本项目采用Coding的代码托管平台，翻译工作将在此平台进行。
我们在Coding创建的项目名为**Chinese_BukkitAPI**(此为私有项目，您必须为成员才能看到此项目)，如您要参与进来，请参阅“如何上传”篇。
##====****翻译规范****====
JavaDoc用来说明某方法/成员变量等的用途.
一般写在某方法/成员变量等的上方.
比如
```java
   /**
     * 简单描述:Gets the {@link Chunk} at the given {@link Location}. 
     * <p>
     * 详细描述: .... 
     * @param location Location of the chunk
     * @return Chunk at the given location
     */
    public Chunk getChunkAt(Location location);
```
分为三部分,第一部分为简述,即简单描述,使用简短的语言描述该东东的用途,
使用.号结尾。 然后在换行后添加换行符<p>(直接换行[[[**无用!!!**]]]).

第二部分为详细描述,用于详细说明方法用途,或举一些简单的例子。**同样使用<p>
换行**。**该部分的最后一行不需要写<p>**。

第三部分为参数说明 param,返回值说明return,抛出异常说明@throws等。
格式:
@param参数：
用法：**@param 参数名 参数说明**
例子：
> @param loc 一个位置({@link Location})
注意！参数名不用翻译，对应的是方法中的参数！

@return参数：
用法：@return 返回值的说明
例子：@return 返回这个类的描述,如果为null则没有描述

@throws参数：
用法：@throws 异常的类名 在什么情况下会抛出这个异常
例子：@throws IllegalArgumentException 如果PlayerListName超过16个字符则抛出
注意千万别把异常的类名丢掉！不然别人不知道会抛出什么异常....

@deprecated参数：
这个参数表示，这个方法已经被新版本弃用了！但是并不代表这个方法会失效或抛
出什么错误之类的（当然也有可能，这个要视情况而定的。一般来说这个都表示这个
方法有什么什么问题，比如安全性问题，所以才被弃用了。或者有其他的办法代替它。比如show方法被弃用了，doc里注明：
@deprecated 这个方法被setVisible(true)方法代替
用法：@deprecated 为什么被弃用/这个方法被什么方法代替了
例子：@deprecated 这个方法被setVisible(true)方法代替
然而...BukkitAPI的javadoc里，使用@deprecated一般是这样的：
@deprecated Magic value (魔法值)
这个magic value的真正含义还不得而知，估计是不安全、新增特性的影响或者其他原因而被弃用。

其中特殊标记{@link 类名}为链接到类名Doc的一个超链接。
还可以使用{@link #方法名(形参列表)}来连!接到某个方法.
如{@link #Chunk getChunkAt(Location location)}

##====****如何翻译****====
翻译以**类/包为单位**.
翻译前请先创建任务（**Coding项目里的任务系统**）,非项目成员请在群里报告，说明将要翻译这个类并查看项目中的这个类是否汉化。
创建任务之前也要检查是否有相同的任务
**检查是否有人跟你一样在翻译这个类/包**

首先翻译请**不要直接机翻**,若使用机翻请**加入自己的理解,并重新组织语言**.
符号除特殊(如简述必须使用.分隔)外,请使用中文标点符号,如 。，；等
换行使用换行符<p> (**不是<br>!**) 除了带参数的比如@return之类的会自动换行.
先在前面写上你的翻译,然后再将原文加上,并在前面加上“原文：”,仅仅对于简述
以及详细描述.
因为简述是写在方法目录中的,所以请先写翻译再在最后加上原文.
```java
   /**
     * 获取某位置({@link Location})所在的区块({@link Chunk})
     * <p>
     * 原文：Gets the {@link Chunk} at the given {@link Location}
     *
     * @param location 给定位置
     * @return 给定位置所在的区块
     */
    public Chunk getChunkAt(Location location);
```
	
对于某些意思不太明确的在群里问,要是真没人知道,在后面加上"?" ,有自己的理解/提醒的,可以加上“译注”
对于某些不懂的或者不太清楚,请在群里问,请不要将"或许吧" "没准"这样的不确定字眼添加到翻译中.
如:
```java
/**
 * 原文：Represents the art on a painting
 * <p>
 * 翻译：....代表绘画艺术？
 * <p>
 * 译注：就是跟画有关的...
 */ 
```
这里是一个标准示例:
```java
/**
* 获取该区块的X轴坐标
* <p>
* 原文:Gets the X-coordinate of this chunk
*
* @return 区块X轴坐标
*/
```
P.S：我们是一个团队，请保持团队合作，争取达到最大的效率 
 
 
##==**如何上传**==
注册Coding(<http://coding.net/>)账号, 将注册邮箱或个性后辍报告给hcrgm ,(**QQ-1769413948**) 添加项目组成员后
进入项目 **<http://coding.net/u/你的个性后辍/p/Chinese_BukkitAPI>** 重新编辑你翻译的类，将你翻译的替换进去.
提示:**整个项目仅能容纳20位成员。**
注:您可以使用**在线编辑/git推送**两种方式上传代码，当然你非要用git的话你的git操作技术必须棒棒哒。