---
title: 'programResource 资源类型 (已弃用) '
description: 表示对作为访问评审目标的对象的引用。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a324c047f6a2a7cf5143d1394696f20c429a12ea
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819732"
---
# <a name="programresource-resource-type-deprecated"></a>programResource 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

**programResource** 对象包含在 [programControl](programcontrol.md) 对象中，表示对作为访问评审目标的对象的引用。

此类型继承自 [标识](identity.md)。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-------- |:---- |:----------- |
| type | String | 资源的类型，指示它是组还是应用。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.programResource"
}-->
```json
{
  "type": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "programResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
