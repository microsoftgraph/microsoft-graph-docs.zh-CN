---
author: tushar20
title: sharePointIdentity 资源类型
ms.localizationpriority: medium
description: 表示SharePoint的标识。
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5f7f92f005e03dbd4403cbdaf1c01f62bd0ac11a
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242360"
---
# <a name="sharepointidentity-resource-type"></a>sharePointIdentity 资源类型

表示 **主角 的 sharePointIdentity。** 

此资源从 **标识** 资源扩展，以提供公开特定于SharePoint的信息（例如 **loginName** 或 SharePoint ID）的能力。

## <a name="properties"></a>属性

| 属性         | 类型                        | 说明 |
|:------------     |:----------------------------|:--------------------------------- |
| displayName      | String                      | 此身份的显示名称。 请注意，这可能并不总是可用或最新的。 例如，如果用户更改其 显示名称，API 可能会在将来的响应中显示新值，但与用户关联的项在使用 [delta](../api/driveitem-delta.md)时不会显示为已更改。 |
| id               | String                      | 身份的唯一标识符。 它可以是一个Azure Active Directory ID，也可以SharePoint ID。 |
| loginName        | String                      | 用户标识的SharePoint名称。 |
| 缩略图       | [thumbnailSet][] 集合 | 包含与 [项关联的 thumbnailSet][] 对象的集合。 有关详细信息，请参阅列出 [driveItem 的缩略图][]。 只读。 可为 Null。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.sharePointIdentity",
  "openType": true,
  "optionalProperties": ["displayName", "thumbnails"]
} -->

```json
{
  "loginName": "string",

  /** inherited from Identity */
  "displayName": "string",
  "id": "string",
  "thumbnails": [{ "@odata.type": "microsoft.graph.thumbnailSet" }]
}
```

[ThumbnailSet]: thumbnailset.md
[列出 driveItem 的缩略图]: ../api/driveitem-list-thumbnails.md

<!-- {
  "type": "#page.annotation",
  "description": "SharePoint Identity contains information about an app, user, or group.",
  "keywords": "sharePointIdentity,loginName, sharePointId, owner, modifier, app, user, group",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/SharePointIdentity"
} -->
