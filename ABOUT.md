## 猫猫的详细概括

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