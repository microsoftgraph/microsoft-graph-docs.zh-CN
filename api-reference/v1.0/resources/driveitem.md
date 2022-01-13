---
author: JeremyKelley
title: DriveItem 资源类型
description: 项目是 OneDrive API 中的主数据模型。每一个都是一个项。
ms.localizationpriority: high
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3be0a329d891bbaccac012b8753a5c374b49a8a7
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61847224"
---
# <a name="driveitem-resource-type"></a>DriveItem 资源类型

命名空间：microsoft.graph

**driveItem** 资源代表文件、文件夹或存储在驱动器中的 其他项。

OneDrive 和 SharePoint 中的所有文件系统对象将作为 **driveItem** 资源返回。 SharePoint 文档库中的项目可以表示为 [listItem][] 或 **driveItem** 资源。

**driveItem** 资源的寻址方式主要有两种：

* 通过 **driveItem** 唯一标识符使用 `drive/items/{item-id}` 的方式
* 通过使用文件系统路径 `/drive/root:/path/to/file` 的方式

有关详细信息，请参阅 [寻址 driveItems](/graph/concepts/onedrive-addressing-driveitems.md)。

**DriveItem** 资源拥有作为属性进行模块化的多个 Facet，用于提供 driveItem 的标识和功能相关数据。例如：

* 文件夹具有 [**folder facet**][folder]
* 文件具有 [**file facet**][file]。
* 除了 file facet 之外，图像还具有 [**image facet**][image]。
* 使用照相机拍摄的图像（照片）具有 [**photo facet**][photo]，用于将项标识为照片，并提供照片的拍摄时间和拍摄所用设备等属性。

具有 **文件夹** Facet 的项目充当项目的容器，因此具有指向文件夹下的 **driveItems** 集合的 `children` 引用。

>**注意：** 在 OneDrive for Business 或 SharePoint 文档库中，如果 **driveItem** 具有 [folder][] Facet，则不返回 **cTag** 属性。

## <a name="methods"></a>方法

| 方法                                                   | 返回类型 | 说明
|:---------------------------------------------------------|:------------|:------------
| [获取项目](../api/driveitem-get.md)                      | driveItem |在驱动器中检索 DriveItem 的元数据。
| [获取分析结果][]                                        | [itemAnalytics][] | 对此资源可获取分析。 
| [按间隔获取活动][]                           | [itemActivityStat][] | 在指定的时间间隔内获取 itemActivityStats 的集合。
| [列出子项](../api/driveitem-list-children.md)       | driveItem 集合 | 在 DriveItem 的子项关系中返回 DriveItems 集合。
| [列出版本](../api/driveitem-list-versions.md)       | [DriveItemVersion][] 集合 | 检索当前用户驱动器中的文件的版本。
| [创建项目](../api/driveitem-post-children.md)         | driveItem | 在指定的驱动器中创建一个 driveItem。
| [更新项目](../api/driveitem-update.md)                | driveItem | 更新驱动器中的 driveItem。
| [上传内容](../api/driveitem-put-content.md)        | driveItem | 将内容上传到 driveItem。
| [下载内容](../api/driveitem-get-content.md)      | 下载 Url | 下载 driveItem 的内容。
| [下载特定文件格式][download-format]         | 下载 Url | 下载具有特定格式的 driveItem 的内容。
| [删除项](../api/driveitem-delete.md)                | 无内容 | 删除 DriveItem。
| [移动项目](../api/driveitem-move.md)                    | driveItem | 将 DriveItem 移动到父项。
| [复制项目](../api/driveitem-copy.md)                    | 有关如何[监视复制操作进度](/graph/long-running-actions-overview)的详细信息。 | 创建 driveItem（包括任何子项）的副本。
| [搜索项目](../api/driveitem-search.md)               | driveItem 集合 | 在项目层次结构中搜索与查询匹配的项目。
| [列出驱动器中的更改](../api/driveitem-delta.md)     | 三角链接 | 列出驱动器中的任何更改。
| [关注项目](../api/driveitem-follow.md)                | driveItem  | 关注 driveItem。
| [取消关注项目](../api/driveitem-unfollow.md)            | 无内容 | 取消关注 driveItem。
| [列出缩略图](../api/driveitem-list-thumbnails.md)   | driveItem 集合 | 使用缩略图列出 driveItems。 
| [创建共享链接](../api/driveitem-createlink.md)    | 共享链接 | 创建共享 driveItem 的链接。
| [添加权限](../api/driveitem-invite.md)            | [权限][]集合 | 向用户发送共享邀请。
| [列出权限](../api/driveitem-list-permissions.md) | [权限][]集合 | 检索 driveItem 上的权限集合。
| [删除权限](../api/permission-delete.md)         | 无内容 | 从 driveItem 中删除权限。
| [获取 WebSocket 频道][getWebSocket]                    | [订阅][] | 使用 socket.io 接收驱动器的近实时更改通知。
| [预览项目][item-preview]                             | json object | 获取项目的短期可嵌入URL以呈现临时预览。
| [签入](../api/driveitem-checkin.md)                  | `POST /drives/{driveId}/items/{itemId}/checkin`
| [签出](../api/driveitem-checkout.md)                | `POST /drives/{driveId}/items/{itemId}/checkout`

## <a name="properties"></a>属性

| 属性             | 类型               | 说明
|:---------------------|:-------------------|:---------------------------------
| audio                | [audio][]          | 音频元数据（如果此项是一个音频文件）。 只读。 仅在 OneDrive 个人版上。
| content              | 流             | 内容流（如果此项表示一个文件）。
| createdBy            | [identitySet][]    | 识别创建项目的用户、设备和应用程序。只读。
| createdDateTime      | DateTimeOffset     | 创建项的日期和时间。只读。
| cTag                 | String             | 项目内容的 eTag。如果只有元数据更改，此 eTag 不会更改。**注意** 如果项目是文件夹，则不返回此属性。只读。
| deleted              | [deleted][]        | 有关项目删除状态的信息。只读。
| description          | String             | 提供该项的对用户可见的说明。读写。仅在 OneDrive 个人版上。
| eTag                 | String             | 整个项目（元数据和内容）的 eTag。只读。
| file                 | [file][]           | 文件元数据（如果此项是一个文件）。只读。
| fileSystemInfo       | [fileSystemInfo][] | 客户端上的文件系统信息。读写。
| folder               | [folder][]         | 文件夹元数据（如果此项是一个文件夹）。只读。
| id                   | String             | 项在驱动器中的唯一标识符。只读。
| image                | [image][]          | 图像元数据（如果此项是一个图像）。只读。
| lastModifiedBy       | [identitySet][]    | 上次修改项目的用户、设备和应用程序的标识。只读。
| lastModifiedDateTime | DateTimeOffset     | 上次修改项目的日期和时间。只读。
| location             | [geoCoordinates][] | 位置元数据（如果此项包含位置数据）。只读。
| 恶意软件 (malware)              | [恶意软件][]        | 恶意软件元数据，如果检测到项目包含恶意软件。只读。
| name                 | String             | 项目名称（文件名和扩展名）。读写。
| package              | [package][]        | 如果存在，则表示此项是一个包，而不是文件夹或文件。包被视为某些上下文中的文件和其他上下文中的文件夹。只读。
| parentReference      | [itemReference][]  | 父信息（如果此项具有父级）。读写。
| pendingOperations    | [pendingOperations][] | 如果存在，则表示可能影响 driveItem 状态的一个或多个操作正在等待完成。只读。
| photo                | [照片][]          | 照片元数据（如果此项包含照片）。只读。
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

>**注意：** ETag 和 cTag 属性在容器（文件夹）中以不同的方式工作。更改任意文件夹后代的内容或元数据时，也会修改 CTag 值。除了从后代派生的属性（例如 **childCount** 或 **lastModifiedDateTime**），仅在更改文件夹的属性时修改 eTag 值。

## <a name="relationships"></a>关系

| 关系       | 类型                        | 说明
|:-------------------|:----------------------------|:--------------------------
| activities         | [itemActivity][] 集合 | 最近发生在此项上的活动的列表。
| 分析          | [itemAnalytics][] 资源  | 此项目上发生的查看活动的相关分析。
| children           | driveItem 集合        | 包含项目直接子项的 Item 对象的集合。仅表示文件夹的项目包含子项。只读。可为 Null。
| createdByUser      | [user][]                    | 创建了项的用户的身份。只读。
| lastModifiedByUser | [user][]                    | 上次修改项的用户的标识。只读。
| listItem           | [listItem][]                | 对于 SharePoint 中的驱动器，关联的文档库列表项。 只读。 可为 null。
| permissions        | [permission][] 集合   | 项目的权限集。只读。可为 Null。
| 订阅      | [订阅][]集合 | 项目上的订阅集。 仅在驱动器根目录上支持。
| 缩略图         | [thumbnailSet][] 集合 | 包含与项目关联的 [ThumbnailSet][] 对象的集合。有关详细信息，请参阅 [获取缩略图][]只读。可为 Null。
| 版本           | [driveItemVersion][] 集合 | 旧版本项的列表。 有关详细信息，请参阅[获取旧版本][]。 只读。 可为 Null。
| 工作簿           | [workbook][]                | 如果是 Excel 工作表文件，访问工作簿 API 可以使用工作表的内容。可为 Null

## <a name="instance-attributes"></a>实例属性

实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。

| 属性名称                     | 类型   | 说明
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | string | 为创建新项目的操作解决冲突的行为。你可以使用值 *fail*、*replace* 或 *rename*。PUT 的默认值是 *replace*。绝不会返回包含该批注的项目。只写。
| @microsoft.graph.downloadUrl      | string | 一个可用于下载此文件的内容的 URL。不需要使用此 URL 进行身份验证。只读。
| @microsoft.graph.sourceUrl        | string | 发出 PUT 请求时，此实例批注可用于指示服务下载 URL 内容并将其存储为文件。只写。

>**注意：** 参数 `@microsoft.graph.conflictBehavior` 应包含在 URL 中，而不是请求正文中。
>
>`@microsoft.graph.downloadUrl` 值是一个短期 URL，不能缓存。 此 URL 在失效前只能使用很短的时间（1 小时）。
删除用户的文件权限可能不会立即使 URL 无效。
>
>OneDrive for Business、SharePoint Online 和 SharePoint Server 2016 [不支持](/onedrive/developer/rest-api/api/driveitem_upload_url?view=odsp-graph-online#remarks&preserve-view=true)使用 `@microsoft.graph.sourceUrl` 属性进行文件上载。

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
  "content": { "@odata.type": "Edm.Stream" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "malware": { "@odata.type": "microsoft.graph.malware" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "pendingOperations": { "@odata.type": "microsoft.graph.pendingOperations" },
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
  "analytics": {"@odata.type": "microsoft.graph.itemAnalytics"},
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "microsoft.graph.driveItemVersion"}],

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

[item-preview]: ../api/driveitem-preview.md
[获取分析结果]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivitystat-getactivitybyinterval.md

[audio]: audio.md
[baseItem]: baseitem.md
[Deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[File]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[获取旧版本]: ../api/driveitem-list-versions.md
[获取缩略图]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[listItem]: listitem.md
[恶意软件]: malware.md
[package]: package.md
[权限]: permission.md
[pendingOperations]: pendingoperations.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[订阅]: subscription.md
[thumbnailSet]: thumbnailset.md
[视频]: video.md
[工作簿]: workbook.md
[user]: /graph/api/resources/users
[publicationFacet]: publicationfacet.md

[DriveItemVersion]: driveitemversion.md
[权限]: permission.md
[订阅]: subscription.md
[itemActivityStat]: itemactivitystat.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
