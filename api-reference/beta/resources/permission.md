---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Permission
localization_priority: Normal
ms.openlocfilehash: e8a4adaa3c1d41270e172f9d0b0e1bf3829927c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344943"
---
# <a name="permission-resource-type"></a>权限资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**权限**资源提供了有关为[driveItem](driveitem.md)资源授予的共享权限的信息。

共享权限具有许多不同的形式。
**权限**资源通过资源上的 facet 表示这些不同的表单。

>**注意:** OneDrive for business 和 SharePoint 文档库不返回**inheritedFrom**属性。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "grantedToIdentities",
    "invitation",
    "inheritedFrom",
    "shareId",
    "expirationDateTime",
    "hasPassword"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.permission"
}-->

```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "grantedToIdentities": [{"@odata.type": "microsoft.graph.identitySet"}],
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string",
  "expirationDateTime": "string (timestamp)",
  "hasPassword": "boolean"
}
```

## <a name="properties"></a>属性

| 属性            | 类型                        | 说明
|:--------------------|:----------------------------|:-------------------------
| id                  | String                      | 在项目的所有权限中，某个权限的唯一标识符。只读。
| grantedTo           | [IdentitySet][]             | 对于用户类型权限，此权限的用户和应用程序的详细信息。只读。
| grantedToIdentities | 集合 ([了解 identityset][]) | 对于链接类型权限, 为其授予权限的用户的详细信息。 只读。
| 邀请          | [SharingInvitation][]       | 此权限的全部关联共享邀请的详细信息。只读。
| inheritedFrom       | [ItemReference][]           | 如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。
| link                | [SharingLink][]             | 如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。
| roles               | 集合（字符串）          | 权限类型，例如 `read`。有关角色的完整列表，请参阅如下内容。只读。
| shareId             | String                      | 可用于通过**[共享 API][]** 访问此共享项的唯一标记。 只读。
| expirationDateTime  | DateTimeOffset              | yyyy-mm-ddthh: MM: ssZ of DateTimeOffset 的格式指示权限的过期时间。 MinValue 指示此权限没有设置过期时间。 可选。
| hasPassword         | Boolean                     | 这指示是否为此权限设置了密码, 它仅显示为 "响应"。 可选和只读, 仅适用于 OneDrive 个人版。

### <a name="roles-enumeration-values"></a>角色枚举值

| 值        | 详细信息                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | 提供读取项的元数据和内容的功能。            |
| `write`     | 提供读取并修改项的元数据和内容的功能。 |
| `sp.owner`  | 对于 SharePoint 和 OneDrive for Business，这表示所有者角色。       |
| `sp.member` | 对于 SharePoint 和 OneDrive for Business，这表示成员角色。      |

permission 资源使用 _Facet_ 说明此资源表示的权限种类。

共享链接包含访问项目所需的唯一标记。

具有 [**Invitation**][SharingInvitation] Facet 的权限表示通过邀请特定用户或组访问文件而添加的权限。

## <a name="sharing-links"></a>共享链接

具有[**链接**][SharingLink] facet 的权限表示在该项上创建的共享链接。
这些是最常见的权限类型。
共享链接提供可用于访问文件或文件夹的唯一 URL。
可以将它们设置为以多种方式授予访问权限。
例如, 您可以使用[createLink][] API 创建一个链接, 该链接适用于登录组织的任何人, 也可以创建可用于任何人的链接, 而无需登录。
您可以使用[invite][] API 创建仅适用于特定人员的链接, 而不管它们是否在贵公司中。

下面是共享链接的一些示例。

### <a name="view-link"></a>查看链接

此视图链接提供对具有该链接的任何人的只读访问权限。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->

```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "scope": "anonymous",
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="edit-link"></a>编辑链接

此编辑链接提供对组织中具有链接的任何人的读取和写入访问权限。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->

```json
{
  "id": "2ceefb3g32hh",
  "roles": ["write"],
  "link": {
    "scope": "organization",
    "type": "edit",
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/fj277ghautbb422707565gnvg23",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="specific-people-link"></a>特定人员链接

此链接提供对`grantedToIdentities`集合中特定人员的读取和写入访问权限。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-people-link" } -->

```json
{
  "id": "3",
  "grantedToIdentities": [
    {
       "user": {
        "id": "35fij1974gb8832",
        "displayName": "Misty Suarez"
      }
    },
    {
       "user": {
        "id": "9397721fh4hgh73",
        "displayName": "Judith Clemons"
      }
    }
  ],
  "roles": ["write"],
  "link": {
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/a577ghg9hgh737613bmbjf839026561fmzhsr85ng9f3hjck2t5s",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="sharing-invitations"></a>共享邀请

[邀请][]API 发送的权限可能在[邀请][SharingInvitation] facet 中有其他信息。
如果邀请发送到与已知帐户不匹配的电子邮件地址, 则在兑换邀请之前 (首次单击该链接并登录时), 可能不会设置**grantedTo**属性。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->

```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

在用户兑换共享邀请后，**grantedTo** 属性将包含兑换权限的帐户的相关信息：

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-redeemed" } -->

```json
{
  "id": "1",
  "roles": ["write"],
  "grantedTo": {
    "user": {
      "id": "5D33DD65C6932946",
      "displayName": "John Doe"
    }
  },
  "invitation": {
    "email": "jd@fabrikam.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

## <a name="methods"></a>方法

| 方法                                                   | REST 路径
|:---------------------------------------------------------|:-----------------------
| [列出权限](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [获取权限](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [创建链接][createLink]                                | `POST /drive/items/{item-id}/createLink`
| [邀请人员][邀请]                                  | `POST /drive/items/{item-id}/invite`
| [更新](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [删除](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[特]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[共享 API]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission",
  "suppressions": []
}
-->
