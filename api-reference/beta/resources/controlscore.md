---
title: " controlScore 资源类型"
description: 此资源包含的租户分数和单个控件的说明。
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042806"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

此资源包含的租户分数和单个控件的说明。

|名称 |类型 |说明 |
|:--|:--|:--|
|   控件名称 |   字符串  |   控件的唯一名称 |
|   分数   |   双精度数  |  租户实现 （它而异逐日控件上的租户操作） 的控件的分数。 |
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
