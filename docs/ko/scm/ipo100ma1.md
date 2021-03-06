# 采购订单登记

## 功能说明


平台中采购订单的登记页面，可自行登记[非交互](../tremItro)型[往来单位](../tremItro)的采购订单，也可以登记[交互](../tremItro)型往来单位的采购订单信息。

> 注意  
> &nbsp;&nbsp;若需要登记交互型往来单位的采购订单信息的话，需要确认:
>
> 1. 相互为交互型往来单位。
> 2. [*物料映射登记*](../base/bpr300ma1)中相关交互型往来单位的[物料映射](../tremIntro)数据。如果商品是从[往来单位店铺](../tremItro)中添加的话，物料映射会自动生成。

---

## 访问路径

*采购订单登记*访问路径：SCM - 采购订单管理 - 采购订单登记

<img :src="$withBase('/images/ko/scm/ipo100ma1-1.jpg')" alt="UNIA3">

---

## 字段说明

* 序号：采购订单详情中顺序号码，注意同一个采购订单中的序号不可重复。
* 物料代码：您公司所登记的物料代码。
* 物料名称：您公司所登记的物料名称。
* 采购单位数量：采购订单对应物料单位的采购数量，支持小数（需配置）。
* 采购单位：采购订单对应物料的采购单位。
* 单价类型：根据不同单价类型选择实际单价和预定单价。
* 采购单价：采购订单对应物料的采购单价。
* 采购金额：不含税采购金额。
* 采购税额：根据不同往来单位设置的税率计算得出。
* 采购总额：采购金额与采购税额的合计。
* 本位币：后缀为本位币的意思是此数据栏显示金额为当前登录公司的公司货币，如接单货币为USD，登录公司本位币为RMB的话，在本位币中会显示USD对应RMB金额，汇率在[*汇率登记*](../base/aba120ma1)中登记。
* 缴税类别：缴税类别中包括缴税、免税。
* 第三方平台：如订单通过OMS拉取的第三方订单则会显示第三方平台名称。
* 第三方订单编号：如订单通过OMS拉取的第三方订单则会显示第三方平台中的订单编号。

---

## 操作方法 - 新增

### **适用于非交互往来单位与交互往来单位**

1.在[主信息](../termIntro)中填写必填项数据。

<img :src="$withBase('/images/ko/scm/ipo100ma1-2.jpg')" alt="UNIA3">

2.点击`添加`按钮，在新增行中填写物料代码、采购单位数量，如需其他详情信息可在相关数据栏中填写相关信息。

<img :src="$withBase('/images/ko/scm/ipo100ma1-3.jpg')" alt="UNIA3">

3.信息确认无误后点击`保存`按钮。

<img :src="$withBase('/images/ko/scm/ipo100ma1-4.jpg')" alt="UNIA3">

4.若要让下一步可以查看到此数据请点击`发布`按钮，将数据发布出去。

### **交互往来单位**

除可点击`添加`按钮添加新的采购订单外，交互往来单位也可以点击`询价参考`查看与往来单位询价信息，选择相应的数据后点击`确定`，信息确认无误后点击`保存`按钮，若要让下一步可以查看到此数据请点击`发布`按钮，将数据发布出去，同时系统会告知往来单位您的采购订单。


## **操作方法 - 查询**

进入页面后直接点击`查询`按钮，输入筛选条件后点击`搜索`，选择想要查看的数据后，点击`应用后关闭`。

> 提示  
> 也可以直接使用`查询上一个`，`查询下一个`按钮快速查询。

<img :src="$withBase('/images/ko/scm/ipo100ma1-5.jpg')" alt="UNIA3">

## **操作方法 - 修改**

查询出数据后，可以点击详情数据进行修改。若订单已发布，则需要`取消发布`后再修改订单。

> 注意  
> 以下几种情况无法修改：  
>
> * 已发布并已在下一步业务中参考了此订单。
> * 已发布并往来单位已参考了此订单。

## **操作方法 - 删除**

查询出数据后，可以点击`全部删除`按钮进行整单删除。若订单已发布，则需要`取消发布`后再删除订单。

> 注意  
> 以下几种情况无法删除：  
>
> * 已发布并已在下一步业务中参考了此订单。
> * 已发布并往来单位已参考了此订单。

---

## **Q&A**

> Q: 往来单位为国外往来单位的税率怎么设置？  
> A: 如果是非交互型往来单位则需要在[*往来单位信息登记*](../base/bcm100ma1)对应的往来单位的详情中查看往来单位所登记的国家、货币、税率等信息。  
>

---

## **相关下一步业务**

* [*采购入库登记*](*)
* [*待入库信息查询*](*)
