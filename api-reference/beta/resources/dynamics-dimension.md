---
title: 维度资源类型
description: Dynamics 365 Business Central 中的维度。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 61666cdaf87e095707e90345128b5ad2cda47426
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071353"
---
# <a name="dimensions-resource-type"></a>维度资源类型

命名空间：microsoft.graph

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



