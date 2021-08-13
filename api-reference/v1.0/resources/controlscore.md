---
title: controlScore 资源类型
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: be1da81848b5669f66735e4288dccd09ccc30ac0384cc66897fb0a501907f031
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202509"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

命名空间：microsoft.graph

包含单个控件的租户分数和说明。

## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|controlName|String|控件的唯一名称。|
|score|双精度|租户获得控件的分数 (因租户对控件控件的操作而异) 。|
|controlCategory|String|控制操作类别 (标识、数据、设备、应用、基础结构) 。|
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

