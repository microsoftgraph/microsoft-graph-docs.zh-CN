---
author: daspek
description: contentTypeOrder 资源指定在选择 UI 中显示内容类型的顺序。
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7198e6f17fc77c73c5b2334bc6d1e7b7262f5dcd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507441"
---
# <a name="contenttypeorder-resource-type"></a>ContentTypeOrder 资源类型

命名空间： microsoft. graph

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

| 属性名称 | 类型    | 说明
|:--------------|:--------|:----------------------------------------------------
| **default**   | boolean | 这是否为默认的内容类型
| **position**  | Int32   | 指定在选择 UI 中显示内容类型的位置。

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
