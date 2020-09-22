---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 964de9f9567c419b4e14d38e79cdff92867fb5ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016805"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

命名空间：microsoft.graph

此资源包含单个控件的租户分数和说明。

|名称 |类型 |说明 |
|:--|:--|:--|
|   controlName |   String  |   控件唯一名称 |
|   分   |   双精度  |  租户实现的控制分数 (根据控件) 上的租户操作，每日变化。 |
|   controlCategory |   String  |  控制操作类别 (标识、数据、设备、应用程序、基础结构) 。 |
|   description |   String  |  控件的说明。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "Double",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


