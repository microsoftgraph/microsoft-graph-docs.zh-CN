---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
ms.openlocfilehash: 34e94128ff3993a01d37770bea1ad046f936405f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341181"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

此资源包含单个控件的租户分数和说明。

|名称 |类型 |说明 |
|:--|:--|:--|
|   controlName |   String  |   控件唯一名称 |
|   score   |   双精度  |  租户实现的控制得分 (根据控件上的租户操作, 每天变化)。 |
|   controlCategory |   String  |  控制措施类别 (标识、数据、设备、应用程序、基础结构)。 |
|   说明 |   String  |  控件的说明。 |

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
