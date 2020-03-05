---
title: 维度资源类型
description: Dynamics 365 Business Central 中的维度。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ed7c7a389778e651af8d2c11c53277a27e022ce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504536"
---
# <a name="dimensions-resource-type"></a>维度资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的维度。

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:-------------|:-------------|:----------|
|[获取尺寸](../api/dynamics-dimension-get.md)|维度|获取一个维。|


## <a name="properties"></a>属性
| 属性           | 类型                  |说明               |
|:-------------------|:----------------------|:-------------------------|
|id                  |GUID                   |项目的唯一 ID。|
|code                |字符串，最大大小为20|维度代码。       |
|displayName         |string                 |指定维度的名称。 此名称将显示在使用该维度的位置。|
|lastModifiedDateTime|datetime               |修改了该维度的最后一个日期/时间。|  


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

