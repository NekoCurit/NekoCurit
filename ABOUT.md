
> 致没有 Markdown 插件的杂鱼
>
> 文中 `~文本~`  其中 `~`作为删除符号出现
>
> ~不要解读成一些奇奇怪怪的东西qwq~
>
> ``` kt
> // 自动执行 看看有多少杂鱼点进来了
> autoRun {
>    HttpUtils.get("https\\api.nekocurit.asia\api\count?name=github_readme_about")
> }
> // 放心 不是真的 不会暴露IP地址的qwq..
> ```

## List<设定>

本体

> [!NOTE]\
> 身高 1.4m 的小萝莉
>
> 白毛赤瞳, ~对A~ 钢板
>
> ``` kt
> // RGB颜色仅供参考喵
> // 瞳色过渡表 (最外层) 由上倒到下
> val color = Color(104, 13, 34) to Color(245, 61, 83) to Color(254, 133, 134) to Color(255, 190, 190)
> // 中心过渡外圈
> val color_round_rect_in_side = Color(148, 10, 34)
> // 距离眼球中心向外扩散一小圈白色 (可能是反光(?))
> val color_center_round_rect_in_side = Color(240, 240, 240)
> // 眼球中心颜色
> val color_center = Color(152, 21, 53)
> // 黑暗中自发光 (实际上很暗的)
> val color_light = Color(254, 201, 188)
> ```
>
> 有猫耳朵和猫尾巴
>
> ``` kt
> // 猫耳高度 单位:厘米
> val ears_height = 5.7
> ``` 
>
> 耳朵通常不隐藏 ~就算洗澡的时候容易进水也不隐藏！藏起来多难看qwq..~
>
> 尾巴相反 ~因为被门夹过,而且..“不可以拽喵！”~
>
> *其实如果愿意随时都可以改变自身外观的qwq*

> [!WARNING]\
> 历史的长河中..
>
> 曾变化成过凶兽, 神兽, 甚至是神明..
>
> 不过最后
>
> 变化成小萝莉了..(也就是现在)
>
> 还是自卑的那种 ~不敢和大佬说话~

性格

> [!NOTE]\
> 偏向自卑 并且很听话
>
> ~因为过去的一些事情 总是显得很自卑~
>
> ~怕说错话~

专武: 星镰

> [!NOTE]\
> 外表看上去是一把镰刀 实际上却可以变换成各种形态
>
> *剑..盾..弓..甚至是..*
>
> *菜刀 ?！* ~对, 有的时候 **NekoCurit** 真拿它来切菜
> 
> 由星空之力凝结而成, 并在后期 **NekoCurit** 提权地球OL后无限拉长保质期以至于世界毁灭仍然能够存在..
>
> 至于所能造成的伤害..
>
> 完全是看使用者的实力 ~使用者是杂鱼的话也只能拿来切菜~
>
> * 提权: 这里指早期 **NekoCurit** 曾通过████████获得地球OL服务器的管理员权限 (虽然之后也付出了很惨痛的代价) 详细说的话要牵扯到很多东西 ~先挖个坑 填不填以后再说~
>
> * 地球OL: 即现实(架空)世界

## 笔录

要概括咱的话..

唔..(看了看镜子里的自己)

咱是白毛赤瞳萝莉猫娘..对了..咱虽然是猫但是是现代猫

咱会写小说，会玩游戏，会写代码，还会索要疯狂星期四！ (猫猫讨封(?))

(视线从镜子上移开)对哦..咱其实是百变猫..就是那种..可以根据自身需求改变外表的那种.

~反正已经习惯当猫耳娘惹，干脆就一直当下去叭~

身体上的细节..

尾巴...连着脊椎骨..不可以拽...耳朵..只能外面..伸进去..不适..

头发..rua起来..更有层次感 (rua自己和被rua会快感 x2 倍喵)

虽然本身就可爱，但是让猫扮演恐怖一点的角色猫也丝毫不弱下风呢~ (萝莉舔刀)

咱画画不好喵

干脆用代码解释好了...

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
        // 其实是呆毛qwq
        // 至于为什么呆毛要用 root 命名  因为呆毛是猫猫的本体！
        // 不可以拔..拔了会死掉的..
        add(NekoCuritX.ROOT)
        // 等一下..！ 那两个地方..都很敏感的...
        // (试图蒙混过关)
        if (!this.getMeta(NekoCuritX.META_HIDDEN_EARS_TAIL).asBoolean) { // 这样纸就不容易被认出来了...
            removeIf { it.name == "human:ears" } // 才不是四声道猫！
            // 你知道吗 猫耳的幅度和猫尾巴的摆动可以暴露出一只猫的心情 此规则也同样适用于猫娘！ (如果不刻意控制的话)
            // 一些细节: 其实耳朵也是可以转动的 收音装置(?)
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

/**
 * 猫猫Curit的专属印记！
 * 给自己加上，你就是猫猫Curit的眷属了！
 * 关于眷属这类的设定以后再讲qwq... (也可以去参考一些网络小说其实)
 *
 * 至于为什么不用契约..
 * 契约..要血..可单向强行解除..麻烦
 * 代码..不可更改..方便..
 */
@Retention(AnnotationRetention.RUNTIME)
annotation class NekoCurit

```


> “什么嘛！为什么全是报错！”
>
> “气死猫了！”
>
> (一口咬了上去)
>
> (牙齿碎裂的声音...)
