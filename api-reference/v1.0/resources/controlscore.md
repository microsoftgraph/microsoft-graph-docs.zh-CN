---
title: controlScore 资源类型
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 64b5377fce01273ab31d7ec293f5dc7a6e1342ff
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629283"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

包含单个控件的租户分数和说明。

## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|controlName|字符串|控制唯一名称。|
|score|双精度|租户实现的控制得分 (根据控件上的租户操作, 每天变化)。|
|controlCategory|字符串|控制措施类别 (标识、数据、设备、应用程序、基础结构)。|
|说明|字符串| 控件的说明。|

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
