---
title: educationExcelResource 资源类型
description: 'educationResource 的子类。 此资源类型代表一个 Excel 文档。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: be9ea1d08575ad9dc07ac9fe538a597da8db2803
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334417"
---
# <a name="educationexcelresource-resource-type"></a>educationExcelResource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md)的子类。 此资源类型代表一个 Excel 文档。  
 
>**注意:** Excel 文件必须位于与此资源所属的 "分配" 或 "提交" 对象相关联的资源文件夹中。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|fileUrl|String|指向 Excel 文件对象的指针。|

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
