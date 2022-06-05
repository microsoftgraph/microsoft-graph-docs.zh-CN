---
author: JeremyKelley
description: 身份资源表示主角的身份。
ms.date: 09/14/2017
title: 标识
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 818fed7343a5af9cd39f0ebc00c43a411089eb96
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899391"
---
# <a name="identity-resource-type"></a>标识资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**身份** 资源表示 _主角_ 的身份。例如，主角可以是用户、设备或应用程序。

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

## <a name="properties"></a>属性

| 属性            | 类型   | 说明                                                                                                                                                                                                                                                                                                           |
|:--------------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName         | String | 此身份的显示名称。请注意，此信息不一定可查看或是最新的。例如，如果用户更改了其显示名称，API 可能会在以后的响应中显示新值，但与用户相关联的项在使用 [delta](../api/driveitem-delta.md) 时不会显示更改后的值。  |
| id                  | String | 身份的唯一标识符。                                                                                                                                                                                                                                                                                   |
| tenantId            | String | 租户的唯一标识 (可选) 。                                                                                                                                                                                                                                                                             |

## <a name="remarks"></a>注解

在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。

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


