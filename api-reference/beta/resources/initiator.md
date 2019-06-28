---
title: 发起程序资源类型
description: 描述启动设置事件的目标或内容。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2846c247d4a0d196d4c620f447b40d47cd486c81
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349358"
---
# <a name="initiator-resource-type"></a>发起程序资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述启动设置事件的目标或内容。 

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|启动设置事件的人员或服务的名称。|
|id|String|唯一标识启动设置事件的人员或服务。|
|initiatorType|String| 发起程序的类型。 可取值为：`user`、`app`、`system`、`unknownFutureValue`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
