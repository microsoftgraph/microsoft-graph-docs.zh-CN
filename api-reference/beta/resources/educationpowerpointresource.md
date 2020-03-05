---
title: educationPowerPointResource 资源类型
description: 'EducationResource 的子类。 这是一种 PowerPoint 资源。 必须将 PowerPoint 文件上传到与**fileResource**目录关联的 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82bd2a49b95bfb8e880869c753556e9cde868236
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501295"
---
# <a name="educationpowerpointresource-resource-type"></a>educationPowerPointResource 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[EducationResource](educationresource.md)的子类。 这是一种 PowerPoint 资源。 必须在与分配或提交相关联的**fileResource**目录中上载 PowerPoint 文件。


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
  "@odata.type": "microsoft.graph.educationPowerPointResource"
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
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
