---
title: educationCategory 资源类型
description: 可应用于分配的类别。
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 49e5f0c27cb643cdba94dc710ae980ef946d19d1
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366105"
---
# <a name="educationcategory-resource-type"></a>educationCategory 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可应用于分配的类别。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Create category](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | 创建新的 **educationCategory**。|
|[获取 educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | 获取现有的 **educationCategory**。|
|[删除类别](../api/educationcategory-delete.md) | 无 | 删除 **educationCategory**。|
|[Get delta](../api/educationcategory-delta.md)|[educationCategory](../resources/educationcategory.md) 集合|获取新创建或更新的 **educationCategory 的** 列表，而无需对集合执行完整读取。|


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String|类别的唯一标识符。|
|displayName|String|类别的唯一标识符。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
