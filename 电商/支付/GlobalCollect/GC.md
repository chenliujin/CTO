* http://www.globalcollect.com/


## 订单确认页


## GC 卡号信息输入页
* 显示订单信息：GetGCOrderCheckoutInfoAction
  * 收货地址：shipping_address
  * 运输方式：shipping_method
  * Product Info
    * product_name
    * quantity
    * model
    * unit_total
  * Order Info
   * Sub Total
   * Shipping Cost
   * Total
* GC UI: ShoppingPayment::GCPaymentProcessor
 * xml 数据模板
 * 替换 xml 中的变量
 * 提交到 GC
 * 显示 GC UI Form

## 支付成功页





## 测试账号
* Visa Credit Cart
* Card No.
 * 4000000000000101
 * 4000000000000002
* Expiration date：大于当前日期
* Security code：随机数字
