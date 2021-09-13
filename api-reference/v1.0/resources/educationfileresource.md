---
title: educationFileResource 资源类型
description: educationResource 的子类，表示与作业或提交关联的文件对象。
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e0e101e1d21bd8e5aa205875a9f444678aeee218
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036639"
---
# <a name="educationfileresource-resource-type"></a>educationFileResource 资源类型

命名空间：microsoft.graph

[educationResource](educationresource.md)的子类，表示与作业或提交关联的文件对象。

在这种情况下，该文件不是 (Word、Excel 等) 特殊文件之一，而是在系统中没有特殊处理的文件。 文件资源必须存储在与此资源所附加到的工作分配或提交关联的 **resourceFolder** 中。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|fileUrl|String|文件资源的磁盘上的位置。|

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


