# 搬瓦工支付宝付款：国内用户扫码付人民币全流程，付款失败怎么办也有解法

搬瓦工（BandwagonHost）买 VPS 最大的门槛从来不是选套餐，而是付款——一家美国主机商，注册界面全英文，结算时能不能直接用支付宝？答案是：可以，但流程里有几个坑，值得提前说清楚。

这篇文章按实际购买顺序走一遍：从注册账户、选套餐、填优惠码，到选择 Alipay 扫码支付人民币，再到付款失败时的几种处理办法，最后附上当前在售的全部套餐价格。所有价格信息基于官网当前页面整理，付款入口见文中各处链接。

## 支付宝能用，这是国内用户最省事的方式

搬瓦工目前支持四种付款方式：PayPal、信用卡、银联、支付宝。对没有国际信用卡、也不想折腾 PayPal 的国内用户来说，支付宝基本是唯一顺滑的选项。

它的实际体验是这样的：

- 结算时按实时汇率自动把美元金额换算成人民币，扫码支付，不需要自己换汇
- 支付宝页面直接显示人民币金额，扣款成功后订单自动激活，一般几分钟内就能收到 VPS 开通邮件
- **30 天内退款原路退回支付宝**，不会强制变成账户余额

搭配优惠码时还剩一个小羊毛可薅。搬瓦工常年有效的循环优惠码（比如 BWH3HYATVBJW，永久循环优惠 6.58%）对支付宝付款同样生效，按下面步骤操作即可：

1. 选套餐、选机房，进入结算页
2. 在 "Promotional Code" 一栏填入优惠码，点击 Validate Code 验证，价格立即刷新
3. 在 Payment Method 里选择 Alipay
4. 点击 Complete Order 生成订单，再点 Make Payment
5. 页面跳转到支付宝，显示 "Pay with Alipay"，扫码或登录付款
6. 扣款成功后回到订单页，等待系统自动开通

整个流程不需要绑卡，不需要外币，手机上的支付宝就能完成。

## 从注册到扫码付款：跟着走一遍

注册和结算都在同一个系统里完成，总共五步。

**第一步，注册账户。** 从搬瓦工官网进入后点击 Register，填写邮箱和密码。邮箱要写真实可用的，开通邮件和后续通知都发到这里。

**第二步，选套餐。** 建议先看完全文后面的套餐表再回来操作，不同套餐能选的机房差别很大。

**第三步，选机房和计费周期。** 这一步最容易花冤枉钱。同款套餐选不同机房价格可能不一样；月付和年付的差价也很大，年付往往比月付划算一半以上。搬瓦工支持在套餐内免费迁移机房，所以拿不准时先选一个，之后还能换。

**第四步，填优惠码。** 上面说过，Validate Code 验证通过后价格才会变化，别填完就走。

**第五步，选 Alipay 付款。** 点击 Complete Order 生成账单后，页面会列出所有支付方式，选择 Alipay，再点击 Make Payment，跳转到支付宝完成扫码即可。

收到开通邮件后，登录 KiwiVM 控制面板就能看到分配好的 IP 和 root 密码，VPS 已经可以使用了。

## 这几种付款失败的情况，都有对应解法

支付宝付款整体顺畅，但搜索"搬瓦工支付宝"的人里，相当一部分是卡在报错才来找答案的。常见的有这几种：

**报错 SECONDARY_MERCHANT_STATUS_ERROR，提示"系统有点儿忙，一会儿再试试"。** 这是最出名的一个。错误码对应的含义是搬瓦工与支付宝之间的商户协议出现了临时问题，不是你的账户被限制，也不是操作错了。这种情况下反复重试没有用，只能等官方与支付宝沟通解决，期间可以换 PayPal 或银联先完成付款。

**点击付款后页面不跳转。** 有时是网络问题，有时是浏览器拦截了跳转。换浏览器、关闭拦截插件、或者直接复制付款链接到新窗口打开，多数能解决。

**付款页面能打开，但支付宝扫码后没有反应。** 先确认订单没有超时，刷新订单页重新生成付款码再试一次。

**PayPal 付款后显示未激活。** 这是 PayPal 的通知延迟问题，付款成功后 VPS 不会立刻开通，等待一段时间会自动同步。

所有这些问题的共同解法是：先确认扣款是否实际发生。如果支付宝已经扣款但订单没激活，联系客服时提供付款凭证即可，钱不会丢。

## 三十天内反悔：退款政策与流程

搬瓦工提供 30 天退款保障，退款会**原路退回支付宝**，不需要手动提供收款账户。但退款有条件，不是所有订单都能全额退：

- 账户注册时间在 30 天以内
- 使用量不超过套餐总量的 10%
- 使用的 VPS 不超过 3 台
- 未使用 SSL 证书等增值服务（这类服务不可退款）
- IP 未被封锁

符合条件时，登录 KiwiVM 后在账单页面提交退款申请即可，一般几个工作日内原路退回。注意两点：域名和 SSL 证书这类附加购买的项目不在退款范围内；超过 30 天的订单不能退款，只能转让或弃用。

## 全套餐对比：先看价格再付款

下面是搬瓦工当前在售的全部 KVM 套餐，人民币金额按实时汇率在支付宝结算时自动换算。表格中的价格是套餐原价，使用循环优惠码还能在此基础上再打折。

| 套餐 | 内存 | CPU | 硬盘 | 流量/月 | 带宽 | 可选机房 | 价格 | 购买 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| KVM PROMO | 1 GB | 2 核 | 20 GB SSD | 1 TB | 1 Gbps | 9 个机房 | $49.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=44) |
| KVM PROMO | 2 GB | 3 核 | 40 GB SSD | 2 TB | 1 Gbps | 9 个机房 | $99.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=45) |
| KVM PROMO | 4 GB | 4 核 | 80 GB SSD | 3 TB | 1 Gbps | 9 个机房 | $19.99/月 或 $199.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=46) |
| KVM PROMO | 8 GB | 5 核 | 160 GB SSD | 4 TB | 1 Gbps | 9 个机房 | $39.99/月 或 $399.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=47) |
| KVM PROMO | 16 GB | 6 核 | 320 GB SSD | 5 TB | 1 Gbps | 9 个机房 | $79.99/月 或 $799.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=48) |
| KVM PROMO | 24 GB | 7 核 | 480 GB SSD | 6 TB | 1 Gbps | 9 个机房 | $119.99/月 或 $1199.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=49) |
| CN2 GIA-E | 1 GB | 2 核 | 20 GB SSD | 1 TB | 2.5 Gbps | 17 个机房 | $49.99/半年 或 $169.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=87) |
| CN2 GIA-E | 2 GB | 3 核 | 40 GB SSD | 2 TB | 2.5 Gbps | 17 个机房 | $89.99/半年 或 $299.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=88) |
| CN2 GIA-E | 4 GB | 4 核 | 80 GB SSD | 3 TB | 2.5 Gbps | 17 个机房 | $56.99/月 或 $549.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=89) |
| CN2 GIA-E | 8 GB | 6 核 | 160 GB SSD | 5 TB | 5 Gbps | 17 个机房 | $86.99/月 或 $879.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=90) |
| CN2 GIA-E | 16 GB | 8 核 | 320 GB SSD | 8 TB | 5 Gbps | 17 个机房 | $159.99/月 或 $1599.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=91) |
| CN2 GIA-E | 32 GB | 10 核 | 640 GB SSD | 10 TB | 10 Gbps | 17 个机房 | $289.99/月 或 $2759.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=92) |
| CN2 GIA-E | 64 GB | 12 核 | 1280 GB SSD | 12 TB | 10 Gbps | 17 个机房 | $549.99/月 或 $5399.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=93) |
| SLA（洛杉矶） | 1 GB | 2 核 | 20 GB NVMe | 1 TB | 2.5 Gbps | 洛杉矶 DC5 | $65.89/季 或 $239.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=164) |
| SLA（洛杉矶） | 2 GB | 3 核 | 40 GB NVMe | 2 TB | 2.5 Gbps | 洛杉矶 DC5 | $116.99/季 或 $399.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=165) |
| SLA（洛杉矶） | 4 GB | 4 核 | 80 GB NVMe | 3 TB | 2.5 Gbps | 洛杉矶 DC5 | $69.99/月 或 $699.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=166) |
| SLA（洛杉矶） | 8 GB | 6 核 | 160 GB NVMe | 5 TB | 5 Gbps | 洛杉矶 DC5 | $109.99/月 或 $1099.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=167) |
| SLA（洛杉矶） | 16 GB | 8 核 | 320 GB NVMe | 8 TB | 5 Gbps | 洛杉矶 DC5 | $199.99/月 或 $1999.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=168) |
| SLA（洛杉矶） | 32 GB | 10 核 | 640 GB NVMe | 10 TB | 10 Gbps | 洛杉矶 DC5 | $369.99/月 或 $3699.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=169) |
| SLA（洛杉矶） | 64 GB | 12 核 | 1280 GB NVMe | 15 TB | 10 Gbps | 洛杉矶 DC5 | $879.99/月 或 $8799.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=170) |
| SLA（洛杉矶） | 64 GB | 12 核 | 1280 GB NVMe | 20 TB | 10 Gbps | 洛杉矶 DC5 | $1159.99/月 或 $11598.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=171) |
| 新加坡 CN2 GIA | 2 GB | 2 核 | 40 GB SSD | 500 GB | 1.5 Gbps | 新加坡 | $49.99/月 或 $499.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=173) |
| 新加坡 CN2 GIA | 4 GB | 4 核 | 80 GB SSD | 1 TB | 1.5 Gbps | 新加坡 | $86.99/月 或 $869.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=174) |
| 新加坡 CN2 GIA | 8 GB | 6 核 | 160 GB SSD | 2 TB | 2.5 Gbps | 新加坡 | $165.99/月 或 $1665.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=175) |
| 新加坡 CN2 GIA | 16 GB | 8 核 | 320 GB SSD | 4 TB | 2.5 Gbps | 新加坡 | $329.99/月 或 $3199.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=176) |
| 新加坡 CN2 GIA | 32 GB | 10 核 | 640 GB SSD | 6 TB | 5 Gbps | 新加坡 | $549.99/月 或 $5549.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=177) |
| 新加坡 CN2 GIA | 64 GB | 12 核 | 1280 GB SSD | 8 TB | 5 Gbps | 新加坡 | $1059.99/月 或 $10559.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=178) |
| 大阪 CN2 GIA | 2 GB | 2 核 | 40 GB SSD | 500 GB | 1.5 Gbps | 大阪 | $49.99/月 或 $499.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=134) |
| 大阪 CN2 GIA | 4 GB | 4 核 | 80 GB SSD | 1 TB | 1.5 Gbps | 大阪 | $86.99/月 或 $869.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=135) |
| 大阪 CN2 GIA | 8 GB | 6 核 | 160 GB SSD | 2 TB | 1.5 Gbps | 大阪 | $165.99/月 或 $1665.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=136) |
| 大阪 CN2 GIA | 16 GB | 8 核 | 320 GB SSD | 4 TB | 1.5 Gbps | 大阪 | $329.99/月 或 $3279.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=137) |
| 大阪 CN2 GIA | 32 GB | 10 核 | 640 GB SSD | 6 TB | 1.5 Gbps | 大阪 | $549.99/月 或 $5549.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=138) |
| 大阪 CN2 GIA | 64 GB | 12 核 | 1280 GB SSD | 8 TB | 1.5 Gbps | 大阪 | $1059.99/月 或 $10559.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=139) |
| 东京 CN2 GIA | 2 GB | 2 核 | 40 GB SSD | 500 GB | 1.2 Gbps | 东京 | $89.99/月 或 $899.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=108) |
| 东京 CN2 GIA | 4 GB | 4 核 | 80 GB SSD | 1 TB | 1.2 Gbps | 东京 | $155.99/月 或 $1559.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=109) |
| 东京 CN2 GIA | 8 GB | 6 核 | 160 GB SSD | 2 TB | 1.2 Gbps | 东京 | $299.99/月 或 $2999.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=110) |
| 东京 CN2 GIA | 16 GB | 8 核 | 320 GB SSD | 4 TB | 1.2 Gbps | 东京 | $589.99/月 或 $5899.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=111) |
| 东京 CN2 GIA | 32 GB | 10 核 | 640 GB SSD | 6 TB | 1.2 Gbps | 东京 | $989.99/月 或 $9989.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=123) |
| 东京 CN2 GIA | 64 GB | 12 核 | 1280 GB SSD | 8 TB | 1.2 Gbps | 东京 | $1889.99/月 或 $18989.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=125) |
| 香港 CN2 GIA | 2 GB | 2 核 | 40 GB SSD | 500 GB | 1 Gbps | 香港 | $89.99/月 或 $899.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=95) |
| 香港 CN2 GIA | 4 GB | 4 核 | 80 GB SSD | 1 TB | 1 Gbps | 香港 | $155.99/月 或 $1559.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=96) |
| 香港 CN2 GIA | 8 GB | 6 核 | 160 GB SSD | 2 TB | 1 Gbps | 香港 | $299.99/月 或 $2999.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=97) |
| 香港 CN2 GIA | 16 GB | 8 核 | 320 GB SSD | 4 TB | 1 Gbps | 香港 | $589.99/月 或 $5899.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=98) |
| 香港 CN2 GIA | 32 GB | 10 核 | 640 GB SSD | 6 TB | 1 Gbps | 香港 | $989.99/月 或 $9989.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=122) |
| 香港 CN2 GIA | 64 GB | 12 核 | 1280 GB SSD | 8 TB | 1 Gbps | 香港 | $1889.99/月 或 $18989.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=124) |
| 迪拜 | 1 GB | 2 核 | 20 GB SSD | 500 GB | 1 Gbps | 迪拜 | $19.99/月 或 $169.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=114) |
| 迪拜 | 2 GB | 3 核 | 40 GB SSD | 1 TB | 1 Gbps | 迪拜 | $32.99/月 或 $299.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=115) |
| 迪拜 | 4 GB | 4 核 | 80 GB SSD | 2 TB | 1 Gbps | 迪拜 | $56.99/月 或 $549.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=116) |
| 迪拜 | 8 GB | 6 核 | 160 GB SSD | 3 TB | 1 Gbps | 迪拜 | $86.99/月 或 $879.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=117) |
| 迪拜 | 16 GB | 8 核 | 320 GB SSD | 4 TB | 1 Gbps | 迪拜 | $159.99/月 或 $1599.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=118) |
| 迪拜 | 32 GB | 10 核 | 640 GB SSD | 5 TB | 1 Gbps | 迪拜 | $289.99/月 或 $2759.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=119) |
| 迪拜 | 64 GB | 12 核 | 1280 GB SSD | 6 TB | 1 Gbps | 迪拜 | $549.99/月 或 $5399.99/年 | [ 查看该套餐](https://bandwagonhost.com/aff.php?aff=79616&pid=120) |

几个选套餐的提示：

- 入门用户选 KVM 1GB 年付就够用，价格是全表最低的一档
- 对国内访问速度有要求，优先看 CN2 GIA 系列，其中 CN2 GIA-E 的机房选择最多、年付价格也最合理
- 香港、东京、新加坡 CN2 GIA 的线路质量最高，但月付起步价也最贵，适合对延迟极度敏感的场景
- 同一套餐月付和年付差距明显，确定长期使用就直接选年付

看中哪个套餐可以直接点表格里的链接进入对应页面，注册后按前面的步骤完成支付宝付款。

## 优惠码怎么填才有效

搬瓦工的优惠码分两种：一种是循环优惠码，续费时继续生效；一种是一次性优惠码，只在首单生效。付款前的结算页面就是填码的地方。

目前公开可试的循环码包括 BWH3HYATVBJW（6.58% 循环优惠）。如果某个码已过期，搬瓦工会显示 "The promotional code you entered is not valid"，这时换一个再试即可，不影响付款流程本身。填码后记得点 Validate Code，看到价格变化才算成功。

## 几个付款前值得确认的细节

**付款货币。** 结算页面显示美元，支付宝扣款时按实时汇率换算成人民币，账单金额以支付宝实际扣款为准。

**自动续费。** 搬瓦工不保存支付方式，也不会自动扣款。套餐到期前会发邮件提醒，需要手动续费。

**退款路径。** 用支付宝付款就退回支付宝，用 PayPal 就退回 PayPal，都走原路，不会变成账户余额强迫你继续消费。

**发票和账单。** 每笔订单在 KiwiVM 后台都有电子账单，可以随时下载。

搬瓦工支付宝付款的整体逻辑就这些：注册、选套餐、填优惠码、选 Alipay、扫码、等开通邮件。付款失败先看错误码，多数情况等一等或者换银联就能解决；30 天内不符合使用预期可以申请原路退款。至于套餐怎么选，预算优先就 KVM 年付，线路优先就 CN2 GIA，表格里的价格和链接都在，按需取用。
