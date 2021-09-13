---
author: JeremyKelley
ms.date: 09/10/2017
title: 身份
ms.localizationpriority: medium
description: 身份资源表示主角的身份。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3165b70282fd3a0a20c373e3c10ca8ab0c6fc909
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098977"
---
# <a name="identity-resource-type"></a>Identity 资源类型

命名空间：microsoft.graph

**身份** 资源表示 _主角_ 的身份。例如，主角可以是用户、设备或应用程序。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity",
  "openType": true,
 "optionalProperties": ["displayName", "thumbnails"] } -->
```json
{
  "displayName": "string",
  "id": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

## <a name="properties"></a>属性

| 属性    | 类型   | 说明                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName | String | 此身份的显示名称。请注意，此信息不一定可查看或是最新的。例如，如果用户更改了其显示名称，API 可能会在以后的响应中显示新值，但与用户相关联的项在使用 [delta](../api/driveitem-delta.md) 时不会显示更改后的值。     |
| id          | String | 身份的唯一标识符。                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a>注解

在某些情况下，角色唯一标识符可能不可用。在这种情况下，将返回身份的 **displayName** 属性，但 **id** 属性将从资源中丢失。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"

} -->

