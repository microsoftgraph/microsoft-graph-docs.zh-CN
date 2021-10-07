---
title: educationExternalResource 资源类型
description: educationResource 的子类。 这是默认资源类型分配服务，用于映射我们不向图形公开的所有资源。 这允许所有 SDK 调用方无缝工作。
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3bfefee10d387a34c783c3f8afec7ee00480a506
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220787"
---
# <a name="educationexternalresource-resource-type"></a>educationExternalResource 资源类型

命名空间：microsoft.graph

表示一个泛型类型，用于映射未在 Microsoft Graph。

继承自 [educationResource](educationresource.md)。

此复杂类型允许所有 SDK 调用方无缝工作。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|WebUrl|String|资源的位置。 必需|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.educationExternalResource"
}-->

```json
{
  "webUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-09-21 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExternalResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
