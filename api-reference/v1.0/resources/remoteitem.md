---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
description: remoteItem 资源指示 driveItem 引用存在于其他驱动器中的项。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0d19034475f72984f023cef368e1fec5f75fe456
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034725"
---
# <a name="remoteitem-resource-type"></a>RemoteItem 资源类型

**remoteItem** 资源指示 [**driveItem**](driveitem.md) 引用存在于其他驱动器中的项。
该资源提供源驱动器和目标项的唯一 ID。

具有非 NULL **remoteItem** facet 的 [**DriveItems**](driveitem.md) 是共享、添加到用户的 OneDrive 的资源，或从项（例如搜索结果）的 hetrogenous 集合返回的项中的资源。

**注意：** 与同一驱动器中的文件夹不同，移动到远程项的 **driveItem** 可更改其 `id` 值。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性名称        | 类型                                | 说明                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [IdentitySet](identityset.md)       | 识别创建项目的用户、设备和应用程序。只读。                                                                                  |
| createdDateTime      | Timestamp                           | 创建项的日期和时间。只读。                                                                                                                        |
| 文件                 | [文件](file.md)                     | 指示远程项是文件。只读。                                                                                                              |
| fileSystemInfo       | [FileSystemInfo](filesysteminfo.md) | 本地文件系统中的远程项的有关信息。只读。                                                                                          |
| 文件夹               | [文件夹](folder.md)                 | 指示远程项是文件夹。只读。                                                                                                            |
| id                   | String                              | 驱动器内远程项的唯一标识符。只读。                                                                                                    |
| lastModifiedBy       | [IdentitySet](identityset.md)       | 上次修改项目的用户、设备和应用程序的标识。只读。                                                                            |
| lastModifiedDateTime | Timestamp                           | 上次修改项目的日期和时间。只读。                                                                                                              |
| name                 | String                              | 可选。远程项的 Filename。只读。                                                                                                                 |
| 包              | [包](package.md)               | 如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。 |
| parentReference      | [ItemReference](itemreference.md)   | 远程项的父级的属性。只读。                                                                                                           |
| shared               | [shared](shared.md)                 | 表示此项已与他人共享，并提供有关项目共享状态的信息。只读。                                       |
| sharepointIds        | [SharepointIds](sharepointids.md)   | 为 OneDrive for Business 和 SharePoint 中的项之间的互操作性提供了完整的项标识符集。只读。                                          |
| size                 | Int64                               | 远程项的大小。只读。                                                                                                                               |
| specialFolder        | [specialFolder][]                   | 如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。                                                                     |
| webDavUrl            | Url                                 | 项的可兼容 DAV 的 URL。                                                                                                                                  |
| WebUrl               | Url                                 | 在浏览器中显示此资源的 URL。只读。                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a>注解

有关 **driveItem** 上 facet 的详细信息，请参阅 [driveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
