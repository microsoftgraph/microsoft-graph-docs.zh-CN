---
title: paymentMethods 资源类型
description: Dynamics 365 Business Central 中的付款方法对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1e4cd044d4b552a9239b742efb302633524ce22b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507243"
---
# <a name="paymentmethods-resource-type"></a>paymentMethods 资源类型
代表 Dynamics 365 Business Central 中的付款方式, 如 PayPal、信用卡和银行帐户。

## <a name="methods"></a>方法

| 方法                                                          | 返回类型  |说明             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[获取 paymentMethods](../api/dynamics-paymentmethods-get.md)      |paymentMethods|获取付款方法对象。   |
|[Post paymentMethods](../api/dynamics-create-paymentmethods.md)  |paymentMethods|创建付款方法对象。|
|[修补程序 paymentMethods](../api/dynamics-paymentmethods-update.md) |paymentMethods|更新付款方法对象。|
|[删除 paymentMethods](../api/dynamics-paymentmethods-delete.md)|无          |删除付款方法对象。|

## <a name="properties"></a>属性
| 属性           | 类型   |说明                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|id                  |GUID    |paymentMethods 的唯一 ID。 不可编辑。           |
|code                |string  |指定付款方法代码。                           |
|displayName         |string  |指定付款方法的显示名称。                   |
|lastModifiedDateTime|datetime|上次修改付款方法的日期/时间。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是 paymentMethods 的 JSON 表示形式。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
