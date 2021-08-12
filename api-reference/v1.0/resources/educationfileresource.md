---
title: educationFileResource 资源类型
description: educationResource 的子类，表示与作业或提交关联的文件对象。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c91b33734ea421c34e3627c76b7dd410ab8d251f262c509b15865d5c8db60814
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146914"
---
# <a name="educationfileresource-resource-type"></a>educationFileResource 资源类型

命名空间：microsoft.graph

[educationResource](educationresource.md)的子类，表示与作业或提交关联的文件对象。

在这种情况下，文件不是 Word、 (Excel 等特殊文件之一) 而是在系统中没有特殊处理的文件。 文件资源必须存储在与此资源所附加到的工作分配或提交关联的 **resourceFolder** 中。

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


