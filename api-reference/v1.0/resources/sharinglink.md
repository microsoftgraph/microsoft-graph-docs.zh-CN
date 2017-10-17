---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingLink
ms.openlocfilehash: 7b7729899d134fa1d5de7debb1f209ec5aadd70d
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="sharinglink-resource-type"></a>SharingLink 资源类型

**SharingLink** 资源将与链接相关的数据项分组到一个单一结构。

如果 [**权限**](permission.md) 资源有一个非 NULL **sharingLink** facet，则该权限表示共享链接（而不是授予给用户或组的权限）。

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
  "type": "view | edit | embed",
  "scope": "anonymous | organization",
  "webHtml": "string",
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性    | 类型          | 说明
|:------------|:--------------|:-------------------------------------
| application | [标识][]  | 链接所关联的应用。
| type        | String        | 创建的链接类型。
| scope       | String        | 由该权限表示的链接范围。值 `anonymous` 表示该链接对任何人均可用，`organization` 表示该链接仅可由登录到同一个租户的用户使用。
| webHtml     | String        | 对于 `embed` 链接，此属性包含在网页中嵌入项的 `<iframe>` 元素的 HTML 代码。
| WebUrl      | String        | 在 OneDrive 网站上的浏览器中打开项的 URL。

[Identity]: identity.md

## <a name="type-enumeration"></a>Type 枚举

此表定义了 **type** 属性的可能值：

| 值   | 角色    | 说明
|:--------|:--------|:---------------------------------------------------------
| `view`  | `read`  | 可查看共享链接，允许只读访问。
| `edit`  | `write` | 授予读写权限的编辑共享链接。
| `embed` | `read`  | 可用于将内容嵌入托管网页的仅供查看共享链接。 OneDrive for Business 或 SharePoint 不支持嵌入链接。

## <a name="scope-enumeration"></a>作用域枚举

| 值          | 说明                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | 任何人均可使用共享链接。                                                                            |
| `organization` | 同一组织（租户）中的任何人均可使用共享链接。不适用于 OneDrive 个人版。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing link facet provides information about how a file is shared.",
  "keywords": "sharing,sharing link, sharing url, webUrl",
  "section": "documentation",
  "tocPath": "Facets/SharingLink"
} -->
