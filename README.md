## 坠于谷底，与世隔绝

「 猫..不想待在容器(Docker)里.. 」

「 猫..想要自由.. 」

## 设定其一 (Normal态)

用户名: NekoCurit / 猫猫Curit

概括自己: 每天活得，云里雾里

一名普普通通的 Minecraft Mod / 插件 开发者.. 

## 设定其二 (Kawaill态)

是白毛！是赤瞳！是萝莉！是猫娘！还是现代猫！

会写小说！会玩游戏！会写代码！还会索要疯狂星期四！ (猫猫索要)

其实是百变猫哦..就是那种..可以根据自身需求改变外表的那种.. ~虽然本质上还是猫娘~

~灵魂本源层已经变不了了 外表变终究是要变回去的~

尾巴...连着脊椎骨..不可以...耳朵..只能外面..一下..

真实实力不强..  ~好欺负 打一拳能哭很久的那种~

喜欢可爱的东西！就像喜欢自己一样

可以从以下方法抓到这只~笨蛋~

> 通过 Telegram   @NekoCurit
> 
>> 直接私聊没关系的哦(容错率非常高的) 闲聊或者是讨论大部分问题..都可以
>>
>> 唔..不喜欢(但可以接受)绕..会绕晕掉.. 
>
>> 可能不太能接受一部分表情/贴纸(大概是具有攻击性的(?))/一部分聊天语气(比如说质问) 在摸清楚之前 还是最好用纯文字聊天qwq 
>
> 通过邮箱 NekoCurit@gmail.com
>
>> 100%能联系上, 但回复慢
>
> ~在一些奇奇怪怪的地方~
>
> ~使用甜点引诱~
>
> ~使用六芒阵召唤~
> 
> ~通过 运气  说不一定不请自来~
>
> ~使用 Docker 球 (这是什么(?)) 捕获

说话风格

``` txt
句中 / 结尾 包含 '(?)'/'(?'   表示不确定 (还是希望说错话不会被大佬挨骂...喵...)
开头 * / 整句用 '()'   额外描述 常用语带场景的角色扮演(?)
结尾 '..?'   直接使用'?'感觉有点不太礼貌(可能 或许是像是质问的语气)  所有换成了这个

结尾 喵   语气助词 (其实根据喵后面的标点符号可以猜出心情)

...

``` 

小愿望

> 希望不看文档反馈不带日志反馈的笨蛋少一点
>
> > 还有那些截屏的 以及那些..拿手机拍屏的
> 
> > 其实猫猫对他们的容忍程度还是很高的qwq... ~毕竟要维持可爱的形象嘛~

> ~被喜欢的人抱回家 养着！~

``` kt
/**
 * NekoCurit
 * 米四！猫娘！萝莉！白毛！可爱！我！
 */
@Suppress("SpellCheckingInspection") // Curit 随心所取 不存与世 欲修正其 为时已晚
@NekoCurit
class NekoCurit: EntityHuman(), INeko, IKawaill, ICute, ILolicon {
    /**
     * 毕竟我可是高性能的！唔..高性能的笨蛋..
     */
    override val priority: Int = Int.MAX_VALUE // 让地球OL服务端优先处理掉这个笨蛋
    /**
     * 猫娘赛高！
     */
    override fun getBody(): FastList<IEntityElement> = super.getBody().apply {
        // 等一下..！ 那两个地方..都很敏感的...
        // (试图蒙混过关)
        if (!this.getMeta(NekoCuritX.META_HIDDEN_EARS_TAIL).asBoolean) { // 这样纸就不容易被认出来了...
            removeIf { it.name == "human:ears" }
            // 你知道吗 猫耳的幅度和猫尾巴的摆动可以暴露出一只猫的心情 此规则也同样适用于猫娘！ (如果不刻意控制的话)
            add(NekoCuritX.CAT_EARS)
            add(NekoCuritX.CAT_TAIL)
        }
    }
    /**
     * 小萝莉是傻傻的存在
     * 不过这..傻过头了！
     * 开玩笑 其实NaN比0好 (目移)
     */
    override fun getIQ(): Float = Float.NaN
}

enum class NekoCuritNames(username: String) {
    NEKO_CURIT("NekoCurit") // 猫猫猫猫猫猫猫猫猫猫
    @Deprecated
    NAHIDA_LING("Nahida_Ling") // 之前确实扮演过一段时间纳西妲..(?) 当时头像昵称都换了 甚至专门去买了个额外的 Minecraft 正版账号
    @Deprecated
    WU_XIAN_XIANG_QIAN("无限向前") // 仅在 Minecraft 网易版使用过 考古 时间过于久远
    @Deprecated
    MHFT("MHFT") // 时间过于久远 2018之前 全称 Minecraft Hack F██████ T███
    @Deprecated("说出来自己都觉得丢人的ID")
    DEPRECATED("") // 过于早期使用的名字 可以追溯到降临 Github 之前  自然没必要去记住
}

/**
 * 猫猫Curit的专属印记！或者...猫猫Curit的眷属！
 * 代码层印记可比契约层强多了qwq...
 */
@Retention(AnnotationRetention.RUNTIME)
annotation class NekoCurit

```
