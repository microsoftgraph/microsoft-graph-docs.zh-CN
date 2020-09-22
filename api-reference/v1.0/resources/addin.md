---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: bbb7a106c3710b5f7e433bfe0c7904f9df91a988
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988588"
---
# <a name="addin-resource-type"></a>addIn 资源类型

命名空间：microsoft.graph

定义使用服务可用于调用特定上下文中的应用的自定义行为。 例如，可以呈现文件流的应用程序 [可能会](/onedrive/developer/file-handlers/?view=odsp-graph-online) 为其 "FileHandler" 功能配置 addIns。 这将使 Microsoft 365 之类的服务在用户正在处理的文档上下文中调用应用程序。

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

