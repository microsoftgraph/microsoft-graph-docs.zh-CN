---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 7f5306f88f2ed14ae13cb95cee7cdb3cfe2ad569405062fe6524b8b747940b9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54190778"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

命名空间：microsoft.graph

此资源包含单个控件的租户分数和说明。

|名称 |类型 |说明 |
|:--|:--|:--|
|   controlName |   String  |   控件唯一名称 |
|   score   |   双精度  |  租户获得控件的分数 (因租户对控件控件的操作而异) 。 |
|   controlCategory |   字符串  |  控制操作类别 (标识、数据、设备、应用、基础结构) 。 |
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


