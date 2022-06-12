---
author: JeremyKelley
title: sharedDriveItem 资源类型
ms.localizationpriority: medium
description: 使用 Shares API 访问共享的 driveItem 时，返回 sharedDriveItem 资源。
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 52fa1c8d4395283f6e33464142eab0f411fd46ac
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034584"
---
# <a name="shareddriveitem-resource-type"></a>sharedDriveItem 资源类型

命名空间：microsoft.graph

使用 [共享](../api/shares-get.md) API 访问共享 [driveItem](driveitem.md) 时，将返回 **sharedDriveItem** 资源。

## <a name="json-representation"></a>JSON 表示形式

下面是 **sharedDriveItem** 资源的 JSON 表示形式。

**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
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
| name     | 字符串                        | 共享项的显示名称。                             |
| 所有者    | [identitySet](identityset.md) | 正在引用的共享项的所有者信息。 |

## <a name="relationships"></a>关系

| 关系名称 | 类型                | 说明
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem]   | 用于访问基础 **driveItem**
| **list**          | [**列表**][list]        | 用于访问基础 **list**
| **listItem**      | [**listItem**][listItem]    | 用于访问基础 **listItem**
| **权限**    | [**许可**][permission] | 用于访问表示基础共享链接的 **权** 限
| **site**          | [**site**][site]        | 用于访问基础 **site**

另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。

| 关系名称 | 类型                         | 说明
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | [**driveItem**][driveItem] 集合 | 共享根中包含的所有 driveItem。 不能枚举此集合。
| **root**          | [**driveItem**][driveItem]   | 用于访问基础 **driveItem**。 已弃用 - 请改用 `driveItem` 。

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a>方法

| 方法                                  | REST 路径                |
| :-------------------------------------- | :----------------------- |
| [获取共享项目](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>注解

有关 DriveItem 上的分面的详细信息，请参阅 [driveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

