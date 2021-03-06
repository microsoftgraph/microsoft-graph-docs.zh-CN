---
title: educationFileResource 资源类型
description: 代表与分配或提交相关联的 file 对象的 educationResource 的子类。  在这种情况下，该文件不是 Word、Excel 等特殊文件 (的) ，而是在系统中没有特殊处理的文件。 文件资源必须存储在与此资源附加到的工作分配或提交相关联的 **resourceFolder** 中。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cafef836f1e6f6fb4c2e379f9b9ad618f2519f72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095438"
---
# <a name="educationfileresource-resource-type"></a>educationFileResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表与分配或提交相关联的 file 对象的 [educationResource](educationresource.md) 的子类。  在这种情况下，该文件不是 Word、Excel 等特殊文件 (的) ，而是在系统中没有特殊处理的文件。 文件资源必须存储在与此资源附加到的工作分配或提交相关联的 **resourceFolder** 中。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|fileUrl|字符串|文件资源在磁盘上的位置。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
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
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


