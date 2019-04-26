---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 107dfb3577489521d2e10e0c8fd2fe52c4f90b10
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341221"
---
# <a name="contenttypeinfo-resource-type"></a>ContentTypeInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**contentTypeInfo** 资源指示项的 SharePoint 内容类型。

## <a name="json-representation"></a>JSON 表示形式

下面是 **contentTypeInfo** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>属性

| 属性名称  | 类型    | 说明
|:---------------|:--------|:--------------------------------------------------
| **id**         | string  | 内容类型的 ID。
| **name**       | string  | 内容类型的名称。

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": []
}
-->
