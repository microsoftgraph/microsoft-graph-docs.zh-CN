---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
ms.openlocfilehash: c303436aafbdbb5167a992f405036b5e00e4d635
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856390"
---
# <a name="sharinglink-resource-type"></a>sharingLink 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**SharingLink**资源组合到单个结构链接相关的数据项。

如果[**权限**](permission.md)资源有一个非空**sharingLink**方面，则权限表示共享链接 （而不是授予用户或用户组的权限）。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": { "@odata.type": "microsoft.graph.identity" },
  "preventsDownload": false,
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性       | 类型          | 说明
|:---------------|:--------------|:-------------------------------------
| application    | [Identity][]  | 链接所关联的应用。
| type           | String        | 创建的链接类型。
| scope          | String        | 由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。
| preventsDownload | 布尔       | 如果为 true 则用户只能使用此链接要在 web 上，查看的项目，并且无法将其用于下载项目的内容。 仅为 OneDrive for Business 和 SharePoint。
| webHtml        | String        | 对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。
| WebUrl         | String        | 在 OneDrive 网站上的浏览器中打开项的 URL。

[Identity]: identity.md

### <a name="type-options"></a>类型选项

下表定义的**type**属性的可能值。

| 值    | 角色     | 说明
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | 可查看共享链接，允许只读访问。
| `edit`   | `write`  | 授予读写权限的编辑共享链接。
| `embed`  | `read`   | 可用于将内容嵌入托管网页的仅供查看共享链接。 OneDrive for Business 或 SharePoint 不支持嵌入链接。

### <a name="scope-options"></a>作用域选项

下表定义的**范围**属性的可能值。

| 值            | Description
|:-----------------|:------------------------------------------------------------
| `anonymous`      | 带链接的任何人都访问，而无需登录。 这可能包括您的组织外部的人员。
| `organization`   | 登录到您的组织 （租户） 的任何人都可以使用以下链接获取的访问权限。 仅在 OneDrive for Business 和 SharePoint 中可用。
| `existingAccess` | 仅已被授予访问通过其他手段项的人员可以访问使用此链接的项目。 仅在 OneDrive for Business 和 SharePoint 中可用。
| `users`          | 链接授予仅对特定列表的人员的访问权限。 仅在 OneDrive for Business 和 SharePoint 中可用。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": ""
}-->
