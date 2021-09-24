---
title: dimensions 资源类型
description: Dynamics 365 Business Central 中的维度。
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: db1a243a9f7eabb8436a6f1ca2b64fe5b74508b5
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508816"
---
# <a name="dimensions-resource-type"></a>维度资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的维度。

## <a name="methods"></a>Methods
| 方法       | 返回类型  |Description|
|:-------------|:-------------|:----------|
|[获取维度](../api/dynamics-dimension-get.md)|dimension|获取维度。|


## <a name="properties"></a>属性
| 属性           | 类型                  |说明               |
|:-------------------|:----------------------|:-------------------------|
|id                  |GUID                   |项目的唯一 ID。|
|code                |字符串，最大大小 20|维度代码。       |
|displayName         |string                 |指定维度的名称。 此名称将显示在使用维度的地方。|
|lastModifiedDateTime|datetime               |上次修改维度的日期/时间。|  


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



