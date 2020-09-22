---
title: taxAreas 资源类型
description: 税务区域。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 140470f0e293b41770779628280f0117d8bb6a89
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027053"
---
# <a name="taxareas-resource-type"></a>taxAreas 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的税务区域资源类型。

## <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 taxAreas](../api/dynamics-taxarea-get.md)|taxAreas|获取税务区域对象。|
|[Post taxAreas](../api/dynamics-create-taxarea.md)|taxAreas|创建税务区域对象。|
|[修补程序 taxAreas](../api/dynamics-taxarea-update.md)|taxAreas|更新税务区域对象。|
|[删除 taxAreas](../api/dynamics-taxarea-delete.md)|无|删除税务区域对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|GUID|税务区域的唯一 ID。 不可编辑。|
|code|字符串，最大大小为20| 税务区域的代码。|
|displayName|字符串，最大大小为50| 税务区域的显示名称。|
|taxType|string|税务区域的税金类型。|
|lastModifiedDateTime|datetime|税区域的最后修改日期时间。 只读。|

## <a name="relationships"></a>关系

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```




