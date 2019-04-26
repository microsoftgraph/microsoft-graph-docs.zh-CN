---
title: educationWordResource 资源类型
description: 'educationResource 的子类。 这是 Word 文档资源。 必须将 Word 文件上载到与**fileResource**目录关联的 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9bd9af22c141991efd85fc240a002b5c7a0eac3b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340193"
---
# <a name="educationwordresource-resource-type"></a>educationWordResource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md)的子类。 这是 Word 文档资源。 必须在与分配或提交相关联的**fileResource**目录中上载 Word 文件。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|fileUrl|String|文件在磁盘上的位置。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
