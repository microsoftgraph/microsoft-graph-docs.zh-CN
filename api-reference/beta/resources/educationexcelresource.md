---
title: educationExcelResource 资源类型
description: 'EducationResource 一个子类。 此资源类型表示 Excel 文档。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 11f28da1f2acaecbdd4f57abe8c6c8a03fbac0f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982370"
---
# <a name="educationexcelresource-resource-type"></a>educationExcelResource 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

[EducationResource](educationresource.md)一个子类。 此资源类型表示 Excel 文档。  
 
>**注意：** Excel 文件必须与此资源所属的工作分配或提交对象关联的资源文件夹中。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|fileUrl|字符串|Excel 文件对象的指针。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
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
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
