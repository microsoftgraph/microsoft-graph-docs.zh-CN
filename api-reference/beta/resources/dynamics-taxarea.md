---
title: taxAreas 资源类型
description: 税务区域。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: aeda0ca136c178355a8a8f9589eb7410399ef62a
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365449"
---
# <a name="taxareas-resource-type"></a>taxAreas 资源类型
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
|code|字符串, 最大大小为20| 税务区域的代码。|
|displayName|字符串, 最大大小为50| 税务区域的显示名称。|
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


