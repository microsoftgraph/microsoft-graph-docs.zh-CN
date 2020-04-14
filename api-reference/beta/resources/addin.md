---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: f20165180db29a0e7157993f5f49d7cfd069f640
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450840"
---
# <a name="addin-resource-type"></a>addIn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义使用服务可用于调用特定上下文中的应用的自定义行为。 例如，可以呈现文件流的应用程序[可能会配置](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online)文件处理程序功能的外接程序。 这将使 Office 365 之类的服务在用户正在处理的文档上下文中调用应用程序。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|containerparentjob||
|properties|[keyValue](keyvalue.md) 集合||
|类型|string||

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
