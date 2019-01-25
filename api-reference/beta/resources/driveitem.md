---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fa172301e633a6f001133d44cb3332a5e133efe2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516740"
---
# <a name="driveitem-resource-type"></a>driveItem 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**driveItem** 资源代表文件、文件夹或存储在驱动器中的 其他项。OneDrive 和 SharePoint 中的所有文件系统对象将作为 **driveItem** 资源返回。

**driveItem** 资源的寻址方式主要有两种：

* 通过 **driveItem** 唯一标识符使用 `drive/items/{item-id}` 的方式
* 通过使用文件系统路径 `/drive/root:/path/to/file` 的方式

**DriveItem** 资源拥有作为属性进行模块化的多个 Facet，用于提供 driveItem 的标识和功能相关数据。例如：

* 文件夹具有[**文件夹 facet**][folder]
* 文件具有[**文件 facet**][file]。
* 除了文件 facet，图像还具有[**图像 facet**][image]。
* 使用照相机拍摄的图像（照片）具有[**照片 facet**][photo]，用于将项标识为照片，并提供照片的拍摄时间和拍摄所用设备等属性。

具有**文件夹** Facet 的项目充当项目的容器，因此具有指向文件夹下的 **driveItems** 集合的 `children` 引用。

## <a name="json-representation"></a>JSON 表示形式

下面是 **driveItem** 资源的 JSON 表示形式。

**driveItem** 资源由 [**baseItem**][baseItem] 派生并继承该资源的属性。

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "baseType": "microsoft.graph.baseItem",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
  "remoteItem": { "@odata.type": "microsoft.graph.remoteItem" },
  "root": { "@odata.type": "microsoft.graph.root" },
  "searchResult": { "@odata.type": "microsoft.graph.searchResult" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "string",

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "content": { "@odata.type": "Edm.Stream" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "Collection(microsoft.graph.driveItemVersion)"}],

  /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "eTag": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": {"@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "string",

  /* instance annotations */
  "@microsoft.graph.conflictBehavior": "string",
  "@microsoft.graph.downloadUrl": "url",
  "@microsoft.graph.sourceUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性             | 类型               | 说明
|:---------------------|:-------------------|:---------------------------------
| audio                | [audio][]          | 音频元数据（如果此项是一个音频文件）。只读。
| createdBy            | [identitySet][]    | 识别创建项目的用户、设备和应用程序。只读。
| createdDateTime      | DateTimeOffset     | 创建项的日期和时间。只读。
| cTag                 | String             | 项目内容的 eTag。如果只有元数据更改，此 eTag 不会更改。**注意** 如果项目是文件夹，则不返回此属性。只读。
| deleted              | [deleted][]        | 有关项目删除状态的信息。只读。
| description          | 字符串             | 提供项的用户可见的说明。读写。仅在 OneDrive 个人版上
| eTag                 | String             | 整个项目（元数据和内容）的 eTag。只读。
| file                 | [file][]           | 文件元数据（如果此项是一个文件）。只读。
| fileSystemInfo       | [fileSystemInfo][] | 客户端上的文件系统信息。读写。
| folder               | [folder][]         | 文件夹元数据（如果此项是一个文件夹）。只读。
| id                   | String             | 项在驱动器中的唯一标识符。只读。
| image                | [image][]          | 图像元数据（如果此项是一个图像）。只读。
| lastModifiedBy       | [identitySet][]    | 上次修改项目的用户、设备和应用程序的标识。只读。
| lastModifiedDateTime | DateTimeOffset     | 上次修改项目的日期和时间。只读。
| location             | [geoCoordinates][] | 位置元数据（如果此项包含位置数据）。只读。
| name                 | String             | 项目名称（文件名和扩展名）。读写。
| package              | [package][]        | 如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。
| parentReference      | [itemReference][]  | 父信息（如果此项具有父级）。读写。
| photo                | [photo][]          | 照片元数据（如果此项包含照片）。只读。
| publication          | [publicationFacet][] | 在支持此类操作的位置提供有关某个项目的已发布或签出状态信息。 默认情况下，不会返回此属性。 只读。 |
| remoteItem           | [remoteItem][]     | 远程项目数据（如果此项是从驱动器共享的项目，而不是被访问的项目）。只读。
| root                 | [root][]           | 如果此属性为非 NULL，则表明 driveItem 是驱动器中最上面的 driveItem。
| searchResult         | [searchResult][]   | 搜索元数据（如果此项目来自搜索结果）。只读。
| shared               | [shared][]         | 表示此项已与他人共享，并提供有关项目共享状态的信息。只读。
| sharepointIds        | [sharepointIds][]  | 返回对 SharePoint REST 兼容性有用的标识符。只读。
| size                 | Int64              | 项目大小，以字节为单位。只读。
| specialFolder        | [specialFolder][]  | 如果当前项同时也是一个特殊的文件夹，则返回此 facet。只读。
| video                | [video][]          | 视频元数据（如果此项是一个视频）。只读。
| WebDavUrl            | String             | 项的可兼容 WebDAV 的 URL。
| WebUrl               | String             | 在浏览器中显示此资源的 URL。只读。

**注意：** ETag 和 cTag 属性在容器（文件夹）中以不同的方式工作。更改任意文件夹后代的内容或元数据时，也会修改 CTag 值。除了从后代派生的属性（例如 **childCount** 或 **lastModifiedDateTime**），仅在更改文件夹的属性时修改 eTag 值。

## <a name="relationships"></a>关系

| 关系       | 类型                            | 说明
|:-------------------|:--------------------------------|:--------------------------
| activities         | [itemActivity][] 集合     | 最近发生在此项上的活动的列表。
| analytics          | [itemAnalytics][] 资源      | 有关此项发生查看活动的分析。
| content            | 流                          | 内容流（如果此项表示一个文件）。
| children           | driveItem 集合            | 包含项目直接子项的 Item 对象的集合。仅表示文件夹的项目包含子项。只读。可为 Null。
| listItem           | [listItem][]                    | 在 SharePoint 中，关联的文档库列表项的驱动器。 只读。 可为 NULL。
| permissions        | [permission][] 集合       | 项目的权限集。只读。可为 Null。
| 缩略图         | [thumbnailSet][] 集合     | 包含与项目关联的 [ThumbnailSet][] 对象的集合。有关详细信息，请参阅 [获取缩略图][]只读。可为 Null。
| 版本           | [driveItemVersion][]集合 | 早期版本的项目列表。 有关详细信息，请参阅[获取早期版本][]。 只读。 可为 NULL。

## <a name="instance-attributes"></a>实例属性

实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。

| 属性名称                     | 类型   | 说明
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | string | 为创建新项目的操作解决冲突的行为。你可以使用值 *fail*、*replace* 或 *rename*。PUT 的默认值是*replace*。绝不会返回包含该批注的项目。只写。
| @microsoft.graph.downloadUrl      | string | 一个可用于下载此文件的内容的 URL。不需要使用此 URL 进行身份验证。只读。
| @microsoft.graph.sourceUrl        | string | 发出 PUT 请求时，此实例批注可用于指示服务下载 URL 内容并将其存储为文件。只写。

**注意：**@Microsoft.graph.downloadUrl 值是短期 URL，并且不能缓存。
URL 期间较短的时间 （1 小时） 之前失效将只能可用。 删除文件的用户权限可能不立即使无效 URL。

## <a name="methods"></a>方法

| 方法                                                   | REST 路径
|:---------------------------------------------------------|:------------------
| [获取项目](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [列出活动](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| [获取分析结果][]                                        | `GET /drive/items/{item-id}/analytics`
| [按间隔获取活动][]                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [列出子项](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [列出版本](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [创建项目](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [更新项目](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [上载内容](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [下载内容](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| [下载特定格式文件][download-format]         | `GET /drive/items/{item-id}/content?format={format}`
| [删除项](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [移动项目](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [复制项目](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [搜索项目](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [列出驱动器中的更改](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [列出缩略图](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [创建共享链接](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [添加权限](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [列出权限](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [删除权限](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| [获取 WebSocket 通道][getWebSocket]                    | `GET /drive/root/subscriptions/socketIo`
| [预览项][item-preview]                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[获取分析结果]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a>注解

在 OneDrive for Business 或 SharePoint 文档库中，如果 **driveItem** 具有[folder][] Facet，则不返回 **cTag** 属性。

[audio]: audio.md
[baseItem]: baseitem.md
[Deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[File]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[获取早期版本]: ../api/driveitem-list-versions.md
[获取缩略图]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[List activities]: ../api/activities-list.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[Shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[thumbnailSet]: thumbnailset.md
[video]: video.md
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": {
    "Resources/Item": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/driveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
