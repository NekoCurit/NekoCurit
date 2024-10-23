## 梦醒之前再抱抱猫猫吧..梦醒之后..就再也抱不到了

## 设定 (文字版)

用户名: NekoCurit

一名普普通通的 Minecraft Mod / MCP / 插件 开发者..

能力不强..

可以从以下方法抓到这只~笨蛋~

> 通过 Telegram   @NekoCurit  (直接私聊没关系的哦)
>
> 通过邮箱 NekoCurit@gmail.com
> 
> ~通过 运气  说不一定不请自来~

## 设定 (代码版)

``` kt
/**
 * NekoCurit
 * 米四！猫娘！萝莉！可爱！我！
 */
@Suppress("SpellCheckingInspection") // Curit 随心所取 不存与世 欲修正其 为时已晚
class NekoCurit: EntityHuman(), INeko, IKawaill, ILolicon {
    /**
     * 毕竟我可是高性能的！唔..高性能的笨蛋..
     */
    override val priority: Int = Int.MAX_VALUE // 让地球OL服务端优先处理掉这个笨蛋
    /**
     * 猫娘赛高！
     */
    override fun getBody(): MutableList<IEntityElement> = super.getBody().apply {
        // 等一下..！ 那两个地方..都很敏感的...
        // (试图蒙混过关)
        if (!this.getMeta(NekoCuritX.META_HIDDEN_EARS_TAIL)) { // 这样纸就不容易被认出来了...
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
    NEKO_CURIT("NekoCurit")
    NAHIDA_LING("Nahida_Ling") // 之前确实扮演过一段时间纳西妲..(?) 当时头像昵称都换了 甚至专门去买了个额外的 Minecraft 正版账号
    @Deprecated("说出来自己都觉得丢人的ID")
    DEPRECATED("") // 过于早期使用的名字 可以追溯到降临 Github 之前  自然没必要去记住
} 
```
~还是尽可能不要在外人面前表现的很脆弱~
