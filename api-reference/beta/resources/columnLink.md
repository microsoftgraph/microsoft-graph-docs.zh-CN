---
author: daspek
description: contentType 上的 columnLink 将网站 columnDefinition 附加到该内容类型。
ms.date: 09/12/2017
title: ColumnLink
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ae75a605f8476b9ec25d5aab5cf50f1bf9508c95
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723526"
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
| **name** | string | 此内容类型中的列的名称。 |

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
