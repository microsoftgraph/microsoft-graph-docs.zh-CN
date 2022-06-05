---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: b749a81b00a1fe93c12fa5b8b17b8e7f95ca89ae
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900184"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

命名空间：microsoft.graph

此资源包含单个控件的租户分数和说明。

|名称 |类型 |说明 |
|:--|:--|:--|
|   controlName |   字符串  |   控制唯一名称 |
|   得分   |   双精度  |  租户实现了控件的分数 (它因控件) 上的租户操作而日复一日地变化。 |
|   controlCategory |   字符串  |  控制操作类别 (标识、数据、设备、应用、基础结构) 。 |
|   description |   字符串  |  控件的说明。 |

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


