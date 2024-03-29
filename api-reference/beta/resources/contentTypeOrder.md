---
author: daspek
description: contentTypeOrder 资源指定在选择 UI 中显示内容类型的顺序。
ms.date: 09/13/2017
title: ContentTypeOrder
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: bf7fca8ae00a0fd131fa2410a980f73fe4588083
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944904"
---
# <a name="contenttypeorder-resource-type"></a>ContentTypeOrder 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**contentTypeOrder** 资源指定在选择 UI 中显示内容类型的顺序。

## <a name="json-representation"></a>JSON 表示形式

下面是 **contentTypeOrder** 资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>属性

| 属性     | 类型    | 说明                                                                   |
| :----------- | :------ | :---------------------------------------------------------------------------- |
| **default**  | boolean | 这是否为默认的内容类型                                      |
| **position** | Int32   | 指定在选择 UI 中显示内容类型的位置。 |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
