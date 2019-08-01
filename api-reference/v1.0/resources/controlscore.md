---
title: controlScore 资源类型
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 68e4bf278b7d1b6ea6f00f75192847abab1ae3a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032842"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

包含单个控件的租户分数和说明。

## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|controlName|String|控制唯一名称。|
|score|双精度|租户实现的控制得分 (根据控件上的租户操作, 每天变化)。|
|controlCategory|String|控制措施类别 (标识、数据、设备、应用程序、基础结构)。|
|说明|String| 控件的说明。|

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
