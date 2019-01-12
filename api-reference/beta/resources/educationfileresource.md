---
title: educationFileResource 资源类型
description: EducationResource 代表相关联的工作分配或提交文件对象的一个子类。  在这种情况下，文件不是一个特殊的文件 （Word、 Excel 和等等），但没有在系统中的特殊处理文件。 文件资源必须存储在与工作分配或提交此资源附加到关联的**资源**。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 96c03dc1571e0f8686116f169706aa35003f92a3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953656"
---
# <a name="educationfileresource-resource-type"></a>educationFileResource 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[EducationResource](educationresource.md)代表相关联的工作分配或提交文件对象的一个子类。  在这种情况下，文件不是一个特殊的文件 （Word、 Excel 和等等），但没有在系统中的特殊处理文件。 文件资源必须存储在与工作分配或提交此资源附加到关联的**资源**。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|fileUrl|字符串|在磁盘上的文件资源的位置。|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
