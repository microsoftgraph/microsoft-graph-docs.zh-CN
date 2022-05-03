---
author: JeremyKelley
description: remoteItem 资源指示 driveItem 引用存在于其他驱动器中的项。
ms.date: 09/10/2017
title: RemoteItem
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 13016aa906c70ed0b3023b9cdd71843243371246
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176522"
---
# <a name="remoteitem-resource-type"></a>RemoteItem 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
  "image" : { "@odata.type": "microsoft.graph.image" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性             | 类型                                | 说明                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [IdentitySet](identityset.md)       | 识别创建项目的用户、设备和应用程序。只读。                                                                                  |
| createdDateTime      | Timestamp                           | 创建项的日期和时间。只读。                                                                                                                        |
| 文件                 | [文件](file.md)                     | 指示远程项是文件。只读。                                                                                                              |
| fileSystemInfo       | [FileSystemInfo](filesysteminfo.md) | 本地文件系统中的远程项的有关信息。只读。                                                                                          |
| 文件夹               | [文件夹](folder.md)                 | 指示远程项是文件夹。只读。                                                                                                            |
| id                   | String                              | 驱动器内远程项的唯一标识符。只读。                                                                                                    |
| image                | [Image](image.md)                   | 图像元数据（如果此项是一个图像）。只读。                                                                                                               |
| lastModifiedBy       | [IdentitySet](identityset.md)       | 上次修改项目的用户、设备和应用程序的标识。只读。                                                                            |
| lastModifiedDateTime | Timestamp                           | 上次修改项目的日期和时间。只读。                                                                                                              |
| name                 | String                              | 可选。远程项的 Filename。只读。                                                                                                                 |
| 包              | [包](package.md)               | 如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。 |
| parentReference      | [ItemReference](itemreference.md)   | 远程项的父级的属性。只读。                                                                                                           |
| shared               | [shared](shared.md)                 | 表示此项已与他人共享，并提供有关项目共享状态的信息。只读。                                       |
| sharepointIds        | [SharepointIds](sharepointids.md)   | 为 OneDrive for Business 和 SharePoint 中的项之间的互操作性提供了完整的项标识符集。只读。                                          |
| size                 | Int64                               | 远程项的大小。只读。                                                                                                                               |
| video                | [Video](video.md)                   | 视频元数据（如果此项是一个视频）。只读。                                                                                                                |
| WebDavUrl            | Url                                 | 项的可兼容 DAV 的 URL。                                                                                                                                  |
| WebUrl               | Url                                 | 在浏览器中显示此资源的 URL。只读。                                                                                                         |

## <a name="remarks"></a>注解

有关 **driveItem** 上 facet 的详细信息，请参阅 [driveItem](driveitem.md)。

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem",
  "suppressions": []
}
-->
