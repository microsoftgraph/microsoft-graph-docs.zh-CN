---
title: addIn 资源类型
description: 下面是资源的 JSON 表示形式。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f54ffcb7404669e593aeda8727325e6ca855140e
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854928"
---
# <a name="addin-resource-type"></a>addIn 资源类型

命名空间：microsoft.graph

定义使用服务可用于调用特定上下文中的应用的自定义行为。 例如，可以呈现文件流的应用程序可能会为 [addIns](/onedrive/developer/file-handlers/?view=odsp-graph-online) 配置其"FileHandler"功能。 这将使 Microsoft 365 之类的服务在用户正在处理的文档上下文中调用应用程序。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|guid||
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
  "id": "GUID",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "String"
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

