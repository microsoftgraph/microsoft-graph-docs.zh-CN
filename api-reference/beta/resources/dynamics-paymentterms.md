---
title: paymentTerms 资源类型
description: Dynamics 365 Business Central 中的付款条款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 1e9e7951da79d524002f004410ef6939d7be5b99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027077"
---
# <a name="paymentterms-resource-type"></a>paymentTerms 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的付款期限。

## <a name="methods"></a>方法

| 方法                                                      | 返回类型|说明            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[获取 paymentTerms](../api/dynamics-paymentterms-get.md)      |paymentTerms|获取付款期限对象。   |
|[Post paymentTerms](../api/dynamics-create-paymentterms.md)  |paymentTerms|创建付款期限对象。|
|[修补程序 paymentTerms](../api/dynamics-paymentterms-update.md) |paymentTerms|更新付款期限对象。|
|[删除 paymentTerms](../api/dynamics-paymentterms-delete.md)|无        |删除付款期限对象。|

## <a name="properties"></a>属性
| 属性                     | 类型     |说明                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|id                            |GUID    |PaymentTerms 的唯一 ID。 不可编辑。           |
|code                          |string  |指定付款期限代码。                           |
|displayName                   |string  |指定付款期限的显示名称。                   |
|dueDateCalculation            |string  |指定用于计算必须进行付款的日期的公式。|
|discountDateCalculation       |string  |指定用于计算要获取折扣付款所必须进行的日期的公式。|
|discountPercent               |数位 |指定针对发票金额的提前付款应用的折扣百分比。|
|calculateDiscountOnCreditMemos|boolean |指定是否应将折扣应用于贷方通知单。 **如果为 True** ，则表示将提供折扣， **false** 表示不会给出折扣。|
|lastModifiedDateTime          |datetime|上次修改 paymentTerms 的日期/时间。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是 paymentTerms 的 JSON 表示形式。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```


