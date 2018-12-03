---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permission
ms.openlocfilehash: 195d4840fdb25339eda3858c0bac2395ee9b1c4a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048302"
---
# <a name="permission-resource-type"></a>权限资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**权限**资源提供有关[driveItem](driveitem.md)资源授予共享权限的信息。

共享权限具有许多不同的形式。
**权限**资源表示这些不同的窗体，通过对资源的方面。

>**注意：** OneDrive for Business 和 SharePoint 文档库不返回**inheritedFrom**属性。

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
| id                  | 字符串                      | 在项目的所有权限中，某个权限的唯一标识符。只读。
| grantedTo           | [IdentitySet][]             | 对于用户类型权限，此权限的用户和应用程序的详细信息。只读。
| grantedToIdentities | 集合 ([IdentitySet][]) | 有关链接类型的权限，向其授予权限的用户的详细信息。 只读。
| 邀请          | [SharingInvitation][]       | 此权限的全部关联共享邀请的详细信息。只读。
| inheritedFrom       | [ItemReference][]           | 如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。
| link                | [SharingLink][]             | 如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。
| roles               | 集合（字符串）          | 权限类型，例如 `read`。有关角色的完整列表，请参阅如下内容。只读。
| shareId             | 字符串                      | 一个可用于访问此**[共享 API][]** 通过共享项目的唯一标记。 只读。
| expirationDateTime  | DateTimeOffset              | 一种格式的 yyyy-MM-ddTHH:mm:ssZ 方法的指示权限的到期时间。 DateTime.MinValue 表示那里无过期期限设置此权限。 可选。
| hasPassword         | 布尔值                     | 这指示是否将密码设置此权限，仅显示响应。 可选只读和仅 OneDrive 个人。

### <a name="roles-enumeration-values"></a>角色枚举值

| 值        | 详细信息                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | 提供读取项的元数据和内容的功能。            |
| `write`     | 提供读取并修改项的元数据和内容的功能。 |
| `sp.owner`  | 对于 SharePoint 和 OneDrive for Business，这表示所有者角色。       |
| `sp.member` | 对于 SharePoint 和 OneDrive for Business，这表示成员角色。      |

permission 资源使用 _Facet_ 说明此资源表示的权限种类。

共享链接包含一个唯一的标记所需访问的项目。

具有 [**Invitation**][SharingInvitation] Facet 的权限表示通过邀请特定用户或组访问文件而添加的权限。

## <a name="sharing-links"></a>共享链接

使用共享对项目创建链接的[**链接**][SharingLink]方面表示的权限。
这些是最常见类型的权限。
共享链接提供了一个可用于访问文件或文件夹的唯一的 URL。
他们可以设置授予多种方式访问权限。
例如，您可以使用[createLink][] API 创建链接的适用于任何人登录到您的组织，或您可以创建适用于任何人，而无需登录的链接。
可以使用[邀请][]API，无论他们是在您的公司或未创建仅适用于特定用户的链接。

下面是共享链接的一些示例。

### <a name="view-link"></a>查看链接

此视图链接与链接的任何人都提供只读访问权限。

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

此编辑链接与链接组织中的任何人都提供读取和写入访问。

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

此链接提供读取和写入访问中的特定人员`grantedToIdentities`集合。

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

发送的[邀请][]API 的权限可能具有[邀请][SharingInvitation]方面中的其他信息。
如果邀请发送给不匹配的已知的帐户的电子邮件地址， **grantedTo**属性可能不设置直到邀请会兑换，其中第一次用户单击的链接并登录时，发生此事件。

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
| [邀请其他人][邀请]                                  | `POST /drive/items/{item-id}/invite`
| [更新](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [删除](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[邀请]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[共享 API]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
