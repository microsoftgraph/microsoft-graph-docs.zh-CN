---
title: currencies 资源类型
description: Dynamics 365 Business Central 中的货币对象
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 228f4c227cd8c0efa5f2ed6dcd885c81a2f5f9ab
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767081"
---
# <a name="currencies-resource-type"></a>currencies 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中使用的货币。

## <a name="methods"></a>方法
| 方法                                                  |返回类型|说明       |
|:--------------------------------------------------------|:----------|:-----------------|
|[获取货币](../api/dynamics-currencies-get.md)      |currencies |获取货币。   |
|[Post currencies](../api/dynamics-create-currencies.md)  |currencies |创建货币。|
|[修补货币](../api/dynamics-currencies-update.md) |currencies |更新货币。|
|[删除货币](../api/dynamics-currencies-delete.md)|无       |删除货币。|

## <a name="properties"></a>属性
| 属性              | 类型   |说明                                                   |
|:----------------------|:-------|:-------------------------------------------------------------|
|id                     |GUID    |货币的唯一 ID。 不可编辑。                  |
|code                   |string  |指定货币代码。                                  |
|displayName            |string  |指定货币显示名称。                          |
|符号                 |string  |指定检查时出现的此货币的符号。|
|amountDecimalPlaces    |string  |指定系统在此货币的金额上显示的小数位数。|
|amountRoundingPrecision|decimal |指定在舍入此货币的金额时所使用的间隔大小。|
|lastModifiedDateTime   |datetime|上次修改货币的日期/时间。 只读。       |  


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

下面是货币的 JSON 表示形式。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "symbol": "string",
  "amountDecimalPlaces": "string",
  "amountRoundingPrecision": "decimal",
  "lastModifiedDateTime": "datetime"
}
```



