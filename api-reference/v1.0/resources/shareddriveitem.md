---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharedDriveItem
ms.openlocfilehash: 3b4497c1a15704388dbb4bb4ba181d3985d65a69
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="shareddriveitem-resource-type"></a>SharedDriveItem 资源类型

使用 [Shares](../api/shares_get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。

## <a name="json-representation"></a>JSON 表示形式

下面是 **sharedDriveItem** 资源的 JSON 表示形式。

**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>属性

| 属性 | 类型                          | 说明                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | String                        | 要访问的内容的唯一标识符。              |
| 名称     | String                        | 共享项的显示名称。                             |
| 所有者    | [IdentitySet](identityset.md) | 正在引用的共享项的所有者信息。 |

## <a name="relationships"></a>关系

| 关系名称 | 类型                | 说明
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem]   | 用于访问基础 **driveItem**
| **list**          | [**list**][list]        | 用于访问基础 **list**
| **listItem**      | [**listItem**][listItem]    | 用于访问基础 **listItem**
| **site**          | [**site**][site]        | 用于访问基础 **site**


另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。

| 关系名称 | 类型                         | 说明
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | [**driveItem**][driveItem] 集合 | 共享根中包含的所有 driveItem。 不能枚举该集合。
| **driveItem**     | [**driveItem**][driveItem]            | 用于访问基础 **driveItem**

[driveItem]: driveItem.md
[list]: list.md
[listItem]: listItem.md
[site]: site.md

## <a name="methods"></a>方法

| 方法                                  | REST 路径                |
| :-------------------------------------- | :----------------------- |
| [获取共享项目](../api/shares_get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>注解

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
