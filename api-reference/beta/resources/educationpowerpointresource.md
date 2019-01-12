---
title: educationPowerPointResource 资源类型
description: 'EducationResource 一个子类。 这是 PowerPoint 资源。 必须在与关联的**fileResource**目录中上载 PowerPoint 文件 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f92d74d8e3dfb7cebcecd607bbd4bd8e2f3b43da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940664"
---
# <a name="educationpowerpointresource-resource-type"></a>educationPowerPointResource 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[EducationResource](educationresource.md)一个子类。 这是 PowerPoint 资源。 必须与工作分配或提交关联的**fileResource**目录中上载 PowerPoint 文件。


## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|fileUrl|字符串|磁盘上的文件的位置。|

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
<!-- {
  "type": "#page.annotation",
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
