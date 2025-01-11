---
title: Wechat of Aur
description: Was aur's WeChat account under attack?
author: AImixAE
date: 2025-1-5 10:07:00 +0800
categories: [Linux]
tags: [arch, aur, wechat]
image:
    path: /assets/img/posts/2025-1-5-Wechat_of_aur/St1.png
---

# Wechat of Aur

元旦我知道的第一个大瓜竟然是 **Aur 中的 Wechat 遭到了恶意攻击**！

## Wechat about kimiblock

维护者 `Kimiblock` 在 `Aur-general` 发布了一个邮件，内容如下：

> Hi,
>
> Recently after the merge of wechat-bin, numerous hostile actions has been taken by some users. I’d request some actions taken against them. The users are listed as follows:
>
> etoyz: Hostile and bad language in AUR comment[a] intentionally misleading other users to disregard the fact that dependencies should better be complete and wechat (formally wechat-uos-bwrap) is partially duplicated by wechat-universal-bwrap. He then suspiciously changes the Chinese ArchWiki[b] and destroyed the wiki’s context. In his questionable merge request, he ignored the fact that universal bwrap lacks dbus proxy and call it “more reasonably”.
>
> gnome: Harassment to the maintainers and their relatives[c].
>
> davy0508: Harassment in a comment[d].
>
> unn: Toxic words in PRQ#68185.
>
> zhaojian: Trolling by filing fake out of date notifications.
>
> Cinnamon, gnomewaylandibus, Xfce, i3WM : Files request with fake reasons, one even started claiming the wechat only works on KDE.
>
> These are not the complete list of hostile users. I hope this situation can be resolved by package maintainers.
>
> [a]: https://aur.archlinux.org/packages/wechat#comment-1004355
> [b]: https://wiki.archlinuxcn.org/wzh/index.php?title=微信&diff=next&oldid=29289
> [c]: https://aur.archlinux.org/packages/wechat#comment-1004526
> [d]: https://aur.archlinux.org/packages/wechat#comment-1004523
>
> --
> Sincerely,
> Kimiblock

该邮件中，`Kimiblock` 声称 `wechcat-bin` 合并后，有一些恶意行为，要求对他们采取行动。其中包括：

- 发布不良评论
- 发布钓鱼信息 _(虚假更新通知)_
- 修改 `Wiki` 内容
- 辱骂维护者及其亲属

这多么令人愤怒！

我尝试与 `Kimiblock` 取得联系，询问他是否可以提供更多信息。这是我与他的邮件:

> 我会积极参与监督工作的
>
> 有问题会及时报告给您
>
> 愿微信战争赶快停止
>
> -- AImixAE@NeoTeak
>
> > Muflone 的主意是拆包纯净版, wechat-bin 目前就是这样的存在. 只不过官方的 Debian 包连 desktop file 都是损坏的, 普通用户还是需要 wechat 以得到一个能用的微信.
> >
> > 不过这样做能稳定闹事者的可能性不高, 还得看事态的发展. 目前我们能做的也只有关注 wiki 是否被恶意修改, 并推动账号封禁.
> >
> > 关于 universal bwrap, 我并不打算近期对它有什么动作. 不过稍后还需要在 wiki 表明它的沙盒有很大漏洞, 甚至未使用 DBus proxy.
> >
> > --
> > Sincerely,
> > Kimiblock
> >
> > > On Jan 1, 2025, at 8:47 PM, AImixAE <AImixAE@outlook.com> wrote:
> > >
> > > 微信很多人都在用，Arch 很多人也在用，两个都用的人也很多，我就是其中之一
> > >
> > > 目前我的微信是通过下载官网的 AppImage 来使用
> > >
> > > 如果 aur 中没有了微信，很多人使用它就会变得很麻烦
> > >
> > > 所以我觉得应该会有很多人关心并且维护这件事情
> > >
> > > 那么我们必须尽快终止这个战争，并且达成一种共识。但这种共识我认为总会有人破坏它
> > >
> > > 因此必须通过其他途径来改变这次微信战争。。。
> > >
> > > 你目前有什么比较好的方法吗？
> > >
> > > （我认为就算是 ban 或者删除这些破坏者的所有账号，他们也会卷土重来，因为傀儡账户太多了）
> > >
> > > （也不敢想象会变成这样）
> > >
> > > > 在 2025/1/1 20:35, Kimiblock Moe 写道:
> > > > AUR 管理员决定如果这场微信战争继续下去, 那么他将会禁止所有微信的打包. 原因为中文用户的破坏力格外大.
> > > >
> > > > --
> > > > Sincerely,
> > > > Kimiblock
> > > >
> > > > > On Jan 1, 2025, at 8:24 PM, AImixAE <AImixAE@outlook.com> wrote:
> > > > >
> > > > > I can't believe that someone in the official WeChat group dares to block WeChat?! What bad things are they doing?
> > > > >
> > > > > I think the wechat in aur is more chaotic, and everyone should consciously form a republican concept, instead of blocking each other for their own bags
> > > > >
> > > > > This should not escalate to a kind of war! I'm complaining about that too.
> > > > >
> > > > > So, if there's anything you need help with, try to let me do it, and I'll do my best!
> > > > >
> > > > > (They're a bunch of holy s\*\*t who block Wechat. One foot flat)
> > > > >
> > > > > 提一嘴：我实在懒得继续翻译成英文了
> > > > >
> > > > > Chinese:
> > > > >
> > > > > 我不敢相信的是，微信官方群的人竟敢拉黑微信？！他们干的都是什么坏事？
> > > > >
> > > > > 我认为 aur 中的 wechat 比较混乱，所有人应该自觉形成一种共和的观念，而不是为了自己的包而互相拉黑
> > > > >
> > > > > 这要上升到一种战争真不应该！我对此也很抱怨。
> > > > >
> > > > > 所以，如果有什么需要帮忙的可以尝试让我来干，我会尽力而为！
> > > > >
> > > > > （拉黑 wechat 的他们就是一群 holy s\*\*t。一脚踩扁）
> > > > >
> > > > > > 在 2025/1/1 17:32, Kimiblock Moe 写道:
> > > > > > Hi AImixAE,
> > > > > >
> > > > > > Thank you for helping me out. This is indeed an uncontrolled situation for me, AUR moderators and other community members.
> > > > > >
> > > > > > The situation is slowly resolving after I had a direct contact with one of the AUR Package Maintainers and I was asked to take control of the wechat-bin pkgbase. We split the package into wechat-bin and wechat. The former one is just purely wechat's own deb package being repackaged, the latter one contains all the fixes one may find useful like HiDPI, Input Method, broken desktop files and such. This action is intended for us to respond to those misbehaving people flooding AUR with some reasons like wechat is not quote unquote pure while actual users can still use the wechat pkgbase for a usable application.
> > > > > >
> > > > > > To ease the pain, we must find the source of those malicious actions. The Qt version of WeChat came out on March and wechat-uos-bwrap, the former pkgbase of wechat is the first to package this new version. It later renamed to wechat-uos-qt and wechat respectively to reduce confusion. Meanwhile, some other people packaged wechat-beta-bwrap (later renamed to wechat-universal-bwrap). We argued about this on the aur-general mailing list and had no real progress at all, due to Chinese moderators too busy to respond and other moderators doesn't know WeChat well. This I'd believe kicked the momentum of duplication because there is really little to no consequences.
> > > > > >
> > > > > > Apart from the root reason for duplication, there's also misleading conversations and maybe harassment going on in WeChat's official QQ group, which was reported by an external source and I have no idea what's going on there. Though most certainly, they have a dedicated group to mislead people to counter wechat and possibly organize a flood attack on AUR using throwaway accounts. These combined with continuous re uploading of wechat-bin has probably caused the PM to contact me directly with a proposal to stop the WeChat war. We'll see if that is effective and if not, packaging of WeChat will get banned on the AUR, which is not I'm hoping for.
> > > > > >
> > > > > > There is little I can do for now though...
> > > > > >
> > > > > > > On 01/01/2025 4:01 pm, AImixAE wrote:
> > > > > > > Hi, how's it going?
> > > > > > >
> > > > > > > I am I'm a questioner on the archlinuxcn bbs.
> > > > > > >
> > > > > > > I recently learned something about wechat-bin. Seeing these contents, I also feel the same way. I don't understand these harassers. But at the same time, I also know how bad these people are.
> > > > > > >
> > > > > > > So I wonder how we should oppose them at the moment. The main thing is to limit them and strengthen community supervision (but it doesn't feel worth it to pay so much for these people)
> > > > > > >
> > > > > > > I also want to contribute something to this thing.
> > > > > > >
> > > > > > > Thanks!
> > > > > > >
> > > > > > > AImixAE

`Kimiblock Moe` 在邮件中详细解释了 `AUR` 上微信打包的情况，包括分包策略、邮件列表讨论和官方 QQ 群的潜在问题。以及 `Kimiblock` 解释了 `Muflone` 的主意和当前的分包策略，并说明还需要关注 `wiki` 修改和账号封禁。等...

但是，一切的受害者只是 `kimiblock` 吗?

## 反面

我在 `archlinuxcn bbs` 上发布了一个主题，以此说明 `wechat-bin` 的恶意攻击

但 `dnn` 表示:

> 作为其中一个不满这个aur维护者行为并且在其中发声的一员，捋一下这个过程。
>
> wechat 原生版未发布的时候有N个wechat包同时在维护，k某在原生版发布之前已经占据了wechat aur包名占位但实际未发布。同时k某在aur-requests中早几个月就请求删除或合并其他微信包。原生版发布后，k某打包了一个实际为 wechat 沙盒版作为 wechat aur 发布，与此同时有其他用户发布了 wechat-bin 打包 wechat 原生版，没有任何修改，发布不久 vote 远超 k某的包。
>
> 我就是最开始在原生版发布后，安装了 wechat 这个包的用户之一。k某维护的挺频繁，但是实际质量非常堪忧，中途几次更新出过不少问题，依赖包频繁变更，期间我使用出现过在前面版本已经设置好的输入法与环境变量缩放在后面的版本就不生效，于是我回头去仔细阅读他 aur build文件内容，发现 wechat 包几乎一个版本一个样，不想作小白鼠于是转向了 wechat-bin。
>
> 在中途某天，k某使用aur规则，合并其他aur包，以我所知 wechat-bin 就是最大受害者，想在 aur 上获得一个 host 资格不可得，可能还有其他几个 wechat 的包被合并到 wechat，不考证了。维护者 @devcom 对于处置不满，删号离去。
>
> 中途存在其他用户自发上传了几次 wechat-bin，均在发布后不久被合并或删除。 wechat-bin 被合并导致不少用户反感并发起了删除 wechat 包的 aur-request，均被 PM 以 invalid reason 否决。后面几次 request中，PM表示 wechat包的问题会得到处理。并且 PM 表示他未看到除了对 k某的反感并未看到任何一个技术性的理由足以使他支持其他用户的请求。
>
> 可能经过 k 某与 pm 的讨论，最终 k 某将 wechat 包一分为2，wechat 和 wechat-bin，wechat-bin 作为微信原生打包，wechat 包留下空壳依赖 wechat-bin 作为沙盒版。现在有用户在 wechat 包中留言，既然 wechat 包不是原装 wechat ，就不要使用 wechat 这个 aur 作为包名，当然可以预期的是，k某处心积虑拿下的 wechat 包想要让他拱手让人怕是痴人说梦，哪怕留下的是挂羊头的改装版 wechat。
>
> 最终结果是 k 某同时控制 wechat 和 wechat-bin，原 wechat-bin 维护者被迫远走 github 自行托管 wechat-bin。
>
> 比较可笑的是 pm 判断包重复的原因是 wechat 和 wechat-bin 下载源为同一个，但是 k 某在合并 wechat-bin 后，中途又将 下载源改为 uos 源，后来有其他用户指出后，或是因为其他我不了解原因，又改回官网下载源。另外 中文arch wiki wechat页是k某的广告位？wechat 中文 wiki ，任何人只要修改了 wiki 上推荐的aur 包，k某最终均会修改为推荐他的 wechat 包。然而 aur 上，更多用户推荐 wechat-universal-bwrap，这里再提一嘴，wechat-universal-bwrap包中途被某个可疑用户提起删除还是合并，wechat-universal-bwrap 包维护者 7Ji 被迫回应并且详列其包存在与 wechat 包不同之处。不知出于什么考虑，wechat-universal-bwrap请求被否决了。幸存者 wechat-universal-bwrap 心有戚戚，已经做好 github 上维护的准备。
>
> 让我刷新认知的是，aur包竟然也会有人想要一手把持，并且 aur 的PM独裁下，用户想要在aur上选择自己使用包的维护者的资格都没有，最终的处理结果竟然是 k 某同时拿下了两个包。假如存在一个k某这样的大神，wiki所谓人人可编辑异变为只能k某可编辑，wiki异化为k某的广告页甚至个人博客，谁能管控这种行为？
>
> 然而到了楼主这里，k某无辜的受到了恶意用户的破坏，problematic 用户在他的包里持续骚扰他和 PM 。
>
> 粪坑一般的简中环境跟离谱的PM处理， PM处于这种睿智的人手上，arch linux 谁爱用谁用吧，我是自觉的滚了。

`kimiblock` 竟然是抢占 `wechat` `wechat-bin` 的人? 为了独裁 `aur` 的微信?!

我不敢相信, 随后 `依云` 也与 `dnn` 讨论起来:

![WechatOfAur2.png](/assets/img/posts/2025-1-5-Wechat_of_aur/St2.png)

![WechatOfAur3.png](/assets/img/posts/2025-1-5-Wechat_of_aur/St3.png)

## In the end

整个 `aur` 环境是多么不公平啊

互相竞争，互相争吵

这真的对吗?

## 引用

1. [archlinuxcn bbs](https://bbs.archlinuxcn.org/viewtopic.php?id=14742)

2. [Wiki](https://wiki.archlinuxcn.org/wiki/%E5%BE%AE%E4%BF%A1)
