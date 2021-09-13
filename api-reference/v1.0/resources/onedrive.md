---
title: 在 Microsoft Graph 中使用文件
description: 可以使用 Microsoft Graph 创建一个跨 OneDrive、OneDrive for Business 和 SharePoint 文档库与文件连接的应用程序。
ms.localizationpriority: high
ms.prod: sharepoint
author: jewan-microsoft
doc_type: conceptualPageType
ms.openlocfilehash: bc3b425a25cb55bdbebbf354a296ac4e9235f047
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062430"
---
# <a name="working-with-files-in-microsoft-graph"></a>在 Microsoft Graph 中使用文件

可使用 Microsoft Graph 创建一个跨 OneDrive、OneDrive for Business 和 SharePoint 文档库与文件连接的应用。通过 Microsoft Graph，可以使用存储在 Microsoft 365 中的文件构建各种体验，从仅存储用户文档到复杂的文件共享方案均可。

Microsoft Graph 公开可用于文件的两个资源类型：

* [驱动器](drive.md) - 表示文件的逻辑容器，例如文档库或用户的 OneDrive。
* [DriveItem](driveitem.md) - 表示驱动器中的项目，例如文档、照片、视频或文件夹。

大部分与文件的交互通过与 **DriveItem** 资源的交互实现。以下是一个 DriveItem 资源示例：

```json
{
  "@content.downloadUrl":"https://public-sn3302.files.1drv.com/y2pcT7OaUEExF7EHOlpTjCE55mIUoiX7H3sx1ff6I-nP35XUTBqZlnkh9FJhWb_pf9sZ7LEpEchvDznIbQig0hWBeidpwFkOqSKCwQylisarN6T0ecAeMvantizBUzM2PA1",
  "createdDateTime": "2016-09-16T03:37:04.72Z",
  "cTag": "aYzpENDY0OEYwNkM5MUQ5RDNEITU0OTI3LjI1Ng",
  "eTag": "aRDQ2NDhGMDZDOTFEOUQzRCE1NDkyNy4w",
  "id":"D4648F06C91D9D3D!54927",
  "lastModifiedBy": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "d4648f06c91d9d3d"
    }
  },
  "name":"BritishShorthair.jpg",
  "size":35212,
  "image":{
    "height":398,
    "width":273
  },
  "file": {
    "hashes":{
      "sha1Hash":"wmgPQ6jrSeMX7JP1XmstQEGM2fc="
    }
  }
}
```

**驱动器** 和 **DriveItem** 资源通过三种不同的方式公开数据：

* _属性_（像 **id** 和 **name**）公开简单的值（字符串、数字、布尔值）。
* _Facet_（像 **文件** 和 **照片**）公开复杂的值。存在的 **文件** 或 **文件夹** Facet 表示 **DriveItem** 的行为和属性。
* _引用_（像 **子项** 和 **缩略图**）指向其他资源的集合。

## <a name="commonly-accessed-resources"></a>经常访问的资源

文件交互的大多数 API 请求将使用以下其中一种基础资源来访问 **驱动器** 或 **DriveItem**。

| 路径                               | 资源
|------------------------------------|-----------------------------------------
| `/me/drive`                        | 用户的 OneDrive
| `/me/drives`                       | 枚举用户可用的 OneDrive 资源。
| `/drives/{drive-id}`               | 通过驱动器 ID 访问特定 **驱动器**。
| `/drives/{drive-id}/root/children` | 枚举特定 **驱动器** 根目录中的 **DriveItem** 资源。
| `/me/drive/items/{item-id}`        | 通过其唯一 ID 访问用户 OneDrive 中的 **DriveItem**。
| `/me/drive/special/{special-id}`   | 通过其已知名称访问用户 OneDrive 中的特殊（命名）文件夹。
| `/users/{user-id}/drive`           | 通过使用用户的唯一标识符访问另一个用户的 OneDrive 。
| `/groups/{group-id}/drive`         | 通过组的唯一 ID 访问组的默认文档库。
| `/shares/{share-id}`               | 通过其 **sharedId** 或共享 URL 访问 **DriveItem**。
| `/sites/{site-id}/drive`           | 访问给定 [SharePoint][] [网站][]的默认 **驱动器**（文档库）
| `/sites/{site-id}/drives`          | 枚举给定 [SharePoint][] [网站][]下的 **驱动器**（文档库）

除了通过唯一 ID 在 **驱动器** 内查找 **DriveItem**，应用还可以通过已知资源中的相对路径查找 **DriveItem**。要使用路径进行查找，请使用冒号 (`:`) 字符对相对路径转义。此表提供了通过不同的方法使用冒号字符来按路径查找项目的示例。

| 路径 | 资源 |
|---|---|
| `/me/drive/root:/path/to/file` | 通过相对于用户的 OneDrive 根文件夹的路径访问 **DriveItem**。 |
| `/me/drive/items/{item-id}:/path/to/file` | 通过相对于另一项的路径访问 **DriveItem**（具有 **文件夹** facet 的 **DriveItem**）。 |
| `/me/drive/root:/path/to/folder:/children` | 通过相对于用户的 OneDrive 根文件夹的路径列出 **DriveItem** 的子项。 |
| `/me/drive/items/{item-id}:/path/to/folder:/children` | 按照相对于另一项的路径列出 **DriveItem** 的子项。 |

## <a name="drive-resource"></a>驱动器资源

[驱动器资源](drive.md) 是用户的 OneDrive 或[ SharePoint][] 文档库内的顶级对象。几乎所有的文件操作都从查找特定驱动器资源开始。

可以通过驱动器的唯一 ID 或 [用户](user.md)、[组](group.md) 或组织的默认驱动器查找驱动器资源。 

## <a name="driveitem-resource"></a>DriveItem 资源

[DriveItems](driveitem.md) 是驱动器文件系统内的对象。访问方法有：使用 `/items/{item-id}` 语法通过其 **id** 访问，或使用 `/root:/path/to/item/` 语法通过其文件系统路径访问。

DriveItems 拥有多个 _Facet_，可提供有关项目标识和功能的数据。

具有 **文件夹** Facet 的 DriveItem 充当项目的容器，并且具有指向文件夹下的项目集合的 **子项** 引用。

## <a name="shared-folders-and-remote-items"></a>共享文件夹和远程项目

OneDrive 个人版用户可以向他们自己的 OneDrive 中添加其他驱动器的一个或多个共享项目。这些共享项目在具有 [remoteItem](remoteitem.md) facet 的 **子项** 集合中显示为 **DriveItem**。

有关使用共享文件夹和远程项目的详细信息，请参阅 [Remote items and shared folders](remoteitem.md)（远程项目和共享文件夹）。

## <a name="sharing-and-permissions"></a>共享和权限

OneDrive 和 SharePoint 文档库最常见的操作之一是与其他人共享内容。Microsoft Graph 使你的应用程序可以创建 [共享链接](../api/driveitem-createlink.md)、[添加权限并发送邀请](../api/driveitem-invite.md) 到驱动器中的项目。

Microsoft Graph 还为应用提供了一种直接从共享链接 [访问共享内容](../api/shares-get.md) 的方法。

## <a name="whats-new"></a>最近更新
了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。

[SharePoint]: sharepoint.md
[网站]: site.md

