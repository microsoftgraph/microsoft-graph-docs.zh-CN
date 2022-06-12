---
author: JeremyKelley
title: sharingLink 资源类型
ms.localizationpriority: medium
description: sharingLink 资源将链接相关的数据项分组到单个结构中。
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 95994292e4925e577c5ffe3dee4edb88fdeaf5a6
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034395"
---
# <a name="sharinglink-resource-type"></a>sharingLink 资源类型

命名空间：microsoft.graph

将链接相关的数据项分组到单个结构中。

如果 [**权限**](permission.md) 资源具有非 null **sharingLink** 方面，则权限表示共享链接 (而不是授予) 人员或组的权限。

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

| 属性    | 类型          | 说明
|:------------|:--------------|:-------------------------------------
| application | [Identity][]  | 链接所关联的应用。
| type        | String        | 创建的链接类型。
| scope       | String        | 由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。
| preventsDownload | 布尔值       | 如果为 true，则用户只能使用此链接来查看 Web 上的项，并且无法使用它来下载项目的内容。 仅适用于OneDrive for Business和SharePoint。
| webHtml     | String        | 对于 `embed` 链接，此属性包含在网页上嵌入项的 `<iframe>` 元素的 HTML 代码。
| WebUrl      | String        | 在 OneDrive 网站上的浏览器中打开项的 URL。

[Identity]: identity.md

## <a name="type-options"></a>类型选项

此表定义了 **type** 属性的可能值：

| 值   | Role    | 说明
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | 可查看共享链接，允许只读访问。
| `edit`  | `write` | 授予读写权限的编辑共享链接。
| `embed` | `read`  | 可用于将内容嵌入托管网页的仅供查看共享链接。 OneDrive for Business 或 SharePoint 不支持嵌入链接。

## <a name="scope-options"></a>范围选项

| 值          | 说明
|:---------------|:------------------------------------------------------------
| `anonymous`    | 拥有该链接的任何人都可以访问，无需登录。 这可能包括组织外部的人员。
| `organization` | 登录到组织（租户）的任何人都可以使用该链接获取访问权限。 仅适用于 OneDrive for Business 和 SharePoint。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(view,edit,embed) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/sharinglink.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization) are in resource, but () are in table"
  ],
  "tocPath": "Facets/SharingLink"
} -->

