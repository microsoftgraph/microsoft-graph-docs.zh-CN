---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/14/2017
title: 身份
localization_priority: Normal
ms.openlocfilehash: a2ba76d5bac372be0a40001028dfb54e690a14fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333667"
---
# <a name="identity-resource-type"></a>标识资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**身份**资源表示_主角_的身份。例如，主角可以是用户、设备或应用程序。

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
| id                  | 字符串 | 身份的唯一标识符。                                                                                                                                                                                                                                                                                   |
| tenantId            | String | 租户的唯一标识 (可选)。                                                                                                                                                                                                                                                                             |

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
