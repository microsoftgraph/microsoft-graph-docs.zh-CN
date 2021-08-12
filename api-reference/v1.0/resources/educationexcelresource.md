---
title: educationExcelResource 资源类型
description: educationResource 的子类。 此资源类型表示Excel文档。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 39f74b488351ddca954db696f9c8ec3bfe5ff97b86d294b5dd2162e199d6c849
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252023"
---
# <a name="educationexcelresource-resource-type"></a>educationExcelResource 资源类型

命名空间：microsoft.graph

educationResource 的 [子类](educationresource.md)。 此资源类型表示Excel文档。  
 
>**注意：** 该Excel文件必须在此资源所属的工作分配或提交对象关联的资源文件夹中。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|fileUrl|String|指向文件Excel指针。|

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
<!--
{
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


