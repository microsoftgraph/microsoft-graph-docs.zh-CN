---
title: " controlScore 资源类型"
description: 此资源包含的租户分数和单个控件的说明。
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891467"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

此资源包含的租户分数和单个控件的说明。

|名称 |类型 |Description |
|:--|:--|:--|
|   控件名称 |   字符串  |   控件的唯一名称 |
|   分数   |   Double  |  租户实现 （它而异逐日控件上的租户操作） 的控件的分数。 |
|   controlCategory |   字符串  |  控制操作类别 （Identity、 数据、 设备、 应用程序、 基础结构）。 |
|   说明 |   字符串  |  控件的说明。 |

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
  "score": "String",
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
