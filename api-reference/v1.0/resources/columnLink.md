---
author: daspek
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
description: contentType 上的 columnLink 将网站 columnDefinition 附加到该内容类型。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4087d97dfec976560bac7c8949d34fd962308950
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240575"
---
# <a name="columnlink-resource-type"></a>ColumnLink 资源类型

命名空间：microsoft.graph

[contentType][] 上的 **columnLink** 将网站 **columnDefinition** 附加到该内容类型。

[contentType]: contenttype.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **columnLink** 资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>属性

| 属性名称 | 类型   | 说明
|:--------------|:-------|:----------------------------------------------------
| **id**        | string | 列的唯一标识符。
| **name**      | string | 此内容类型中的列的名称。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->

