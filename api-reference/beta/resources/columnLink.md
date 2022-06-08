---
author: daspek
description: contentType 上的 columnLink 将网站 columnDefinition 附加到该内容类型。
ms.date: 09/12/2017
title: ColumnLink
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8bf46496209b62748c82e46ca52ec7e7e80ded7c
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944946"
---
# <a name="columnlink-resource-type"></a>ColumnLink 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。

[contentType]: contenttype.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **columnLink** 资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name&quot;: &quot;string"
}
```

## <a name="properties"></a>属性

| 属性 | 类型   | 说明                                   |
| :------- | :----- | :-------------------------------------------- |
| **id**   | string | 列的唯一标识符。         |
| **名称** | string | 此内容类型中的列的名称。 |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": []
}
-->
