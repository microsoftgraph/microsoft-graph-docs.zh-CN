---
author: JeremyKelley
title: 标识资源类型
description: 表示执行组件的标识。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 80c48a178bcc2e82848d245df3383e792eec01f3
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855873"
---
# <a name="identity-resource-type"></a>标识资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 _执行组件_ 的标识。 例如，主角可以是用户、设备或应用程序。

在某些情况下，执行组件的唯一标识符可能不可用。 在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。

## <a name="properties"></a>属性

| 属性            | 类型   | 说明                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName         | String | 标识的显示名称。 请注意，这可能并不总是可用或最新。 例如，如果用户更改其显示名称，则 API 可能会在将来的响应中显示新值，但与用户关联的项目在使用 [增量](../api/driveitem-delta.md)时不会显示为已更改。  |
| id                  | String | 身份的唯一标识符。                                                                                                                                                                                                                                                                                   |
| tenantId            | String | 租户的唯一标识 (可选) 。                                                                                                                                                                                                                                                                             |

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity", "optionalProperties": ["displayName", "tenantId", "thumbnails"], "openType": true } -->

```json
{
  "displayName": "string",
  "id": "string",
  "tenantId": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity",
  "suppressions": []
}
-->


