---
author: JeremyKelley
description: SharingLink 资源将与链接相关的数据项分组到一个单一结构中。
ms.date: 09/10/2017
title: SharingLink
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e96164b636866637a30f733cb46da5124d90fa49
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520644"
---
# <a name="sharinglink-resource-type"></a>sharingLink 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**SharingLink**资源将与链接相关的数据项分组到一个单一结构中。

如果[**权限**](permission.md)资源具有非 null **sharingLink** facet，则该权限表示共享链接（而不是授予给个人或组的权限）。

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
| scope          | 字符串        | 由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。
| preventsDownload | 布尔       | 如果为 true，则用户只能使用此链接查看 web 上的项目，并且无法使用它下载项目的内容。 仅适用于 OneDrive for Business 和 SharePoint。
| webHtml        | String        | 对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。
| webUrl         | String        | 在 OneDrive 网站上的浏览器中打开项的 URL。

[Identity]: identity.md

### <a name="type-options"></a>类型选项

下表定义了**type**属性的可能值。

| 值    | Role     | 说明
|:---------|:---------|:---------------------------------------------------------
| `view`   | `read`   | 可查看共享链接，允许只读访问。
| `edit`   | `write`  | 授予读写权限的编辑共享链接。
| `embed`  | `read`   | 可用于将内容嵌入托管网页的仅供查看共享链接。 OneDrive for Business 或 SharePoint 不支持嵌入链接。

### <a name="scope-options"></a>作用域选项

下表定义了**scope**属性的可能值。

| 值            | 说明
|:-----------------|:------------------------------------------------------------
| `anonymous`      | 拥有该链接的任何人都可以访问，无需登录。 这可能包括组织外部的人员。
| `organization`   | 登录到组织（租户）的任何人都可以使用该链接获取访问权限。 仅适用于 OneDrive for Business 和 SharePoint。
| `existingAccess` | 只有已通过其他方式授予对项目的访问权限的人员才能使用此链接访问项目。 仅适用于 OneDrive for Business 和 SharePoint。
| `users`          | 链接仅向特定人员列表授予访问权限。 仅适用于 OneDrive for Business 和 SharePoint。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
