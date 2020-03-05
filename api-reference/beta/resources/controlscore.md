---
title: " controlScore 资源类型"
description: 此资源包含单个控件的租户分数和说明。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f718e197e690d3779870e5996161461fe8f60915
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507413"
---
#  <a name="controlscore-resource-type"></a>controlScore 资源类型

命名空间： microsoft. graph

此资源包含单个控件的租户分数和说明。

|名称 |类型 |说明 |
|:--|:--|:--|
|   controlName |   String  |   控件唯一名称 |
|   score   |   双精度  |  租户实现的控制得分（根据控件上的租户操作，每天变化）。 |
|   controlCategory |   String  |  控制措施类别（标识、数据、设备、应用程序、基础结构）。 |
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
