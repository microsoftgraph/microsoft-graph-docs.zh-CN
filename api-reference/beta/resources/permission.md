---
author: JeremyKelley
title: permission 资源类型
description: 表示为 driveItem 授予的共享权限的权限资源
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a96e86f230f01315d047e8f1ad40b910dd760b65
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61241658"
---
# <a name="permission-resource-type"></a>permission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

permission 资源提供有关为[driveItem](driveitem.md)资源授予的共享权限的信息。

共享权限具有许多不同的形式。
权限 **资源** 通过资源上的 Facet 表示这些不同的形式。

>**注意：OneDrive for Business** 和SharePoint库不会返回 **inheritedFrom** 属性。

OneDrive for Business 和 SharePoint 文档库不返回 **inheritedFrom** 属性。
**grantedTo** 和 **grantedToIdentities** 将下一步弃用，响应将在相应的属性名称下分别迁移到 **grantedToV2** 和 **grantedToIdentitiesV2。**

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "grantedToIdentities",
    "grantedToV2",
    "grantedToIdentitiesV2",
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
  "grantedToV2": {"@odata.type": "microsoft.graph.sharePointIdentitySet"},
  "grantedToIdentitiesV2": [{"@odata.type": "microsoft.graph.sharePointIdentitySet"}],
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

| 属性                         | 类型                                      | 说明 |
|:---------------------------------|:------------------------------------------|:------------------------- |
| id                               | String                                    | 在项目的所有权限中，某个权限的唯一标识符。只读。 |
| grantedToV2                      | [SharePointIdentitySet][]                 | 对于用户类型权限，此权限的用户和应用程序的详细信息。 只读。 |
| grantedToIdentitiesV2            | [SharePointIdentitySet (集合][])      | 对于链接类型权限，被授予权限的用户的详细信息。只读。 |
| 邀请                       | [SharingInvitation][]                     | 此权限的全部关联共享邀请的详细信息。只读。 |
| inheritedFrom                    | [ItemReference][]                         | 如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。 |
| link                             | [SharingLink][]                           | 如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。 |
| 角色                            | 集合（字符串）                        | 权限的类型，例如 `read` ， 。 有关角色的完整列表，请参阅如下内容。 只读。 |
| shareId                          | String                                    | 可通过 **[共享 API][]** 访问此共享项目的唯一令牌。只读。 |
| expirationDateTime               | DateTimeOffset                            | DateTimeOffset 的格式 yyyy-MM-ddTHH:mm:ssZ 表示权限的过期时间。 DateTime.MinValue 表示此权限没有设置过期时间。 可选。 |
| HasPassword                      | 布尔值                                   | 指示是否为此权限设置了密码。 此属性只出现在响应中。 可选。 只读。 仅OneDrive个人。 |
| grantedTo (弃)            | [IdentitySet](identityset.md)             | 对于用户类型权限，此权限的用户和应用程序的详细信息。 只读。 |
| grantedToIdentities (已弃)  | Collection([IdentitySet](identityset.md)) | 对于类型权限，是已授予权限的用户的详细信息。 只读。 |

### <a name="roles-property-values"></a>角色属性值

| 值           | 说明                                                                    |
|:----------------|:-------------------------------------------------------------------------------|
| 阅读            | 提供读取项的元数据和内容的功能。            |
| 写入           | 提供读取并修改项的元数据和内容的功能。 |
| 所有者           | 对于 SharePoint 和 OneDrive for Business，这表示所有者角色。       |

权限资源使用 _facet_ 提供有关由该资源表示的权限类型的信息。

共享链接包含访问该项所需的唯一令牌。

具有 [**邀请**][SharingInvitation] facet 的权限表示通过邀请特定用户或组访问文件而添加的权限。

## <a name="sharing-links"></a>共享链接

具有 [**链接**][SharingLink] facet 的权限表示在该项上创建的共享链接。
这些是最常见的权限类型。
共享链接提供可用于访问文件或文件夹的唯一 URL。
可将其设置为通过多种方式授予访问权限。
例如，可使用 [createLink][] API 创建适用于已登录到组织的任何用户的链接，或创建可用于任何人且无需登录的链接。
你可以使用 [invite][] API 创建仅适用于特定人员的链接（无论他们是否在你的公司中）。

下面是一些共享链接示例。

### <a name="view-link"></a>查看链接

此查看链接向具有相应链接的任何人提供只读访问权限。

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

此编辑链接向组织中具有相应链接的任何人提供读写访问权限。

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

### <a name="existing-access-link"></a>现有的访问链接

此链接不会向用户授予任何其他特权。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-existing-link" } -->

```json
{
  "id": "00000000-0000-0000-0000-000000000000",
  "roles": ["read"],
  "link": {
    "scope": "existingAccess",
    "type": "view",
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/Shared%20Documents/SampleDoc.docx?d=w12345",
  },
  "expirationDateTime": "0001-01-01T00:00:00Z"
}
```

### <a name="specific-people-link"></a>特定人员链接

此链接向 `grantedToIdentities` 集合中的特定人员提供读写访问权限。

<!-- {"blockType": "example", truncated: true, "@odata.type": "microsoft.graph.permission", "name": "permission-people-link" } -->

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
  "grantedToIdentitiesV2": [
    {
       "user": {
        "id": "35fij1974gb8832",
        "displayName": "Misty Suarez"
      },
      "siteUser": {
        "id": "1",
        "displayName": "Misty Suarez",
        "loginName": "Misty Suarez"
      }
    },
    {
       "user": {
        "id": "9397721fh4hgh73",
        "displayName": "Judith Clemons"
      },
      "siteUser": {
        "id": "2",
        "displayName": "Judith Clemons",
        "loginName": "Judith Clemons"
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

邀请或授予 API[][]发送[][]的权限可以在邀请[][SharingInvitation] Facet 中包含与已知帐户不匹配的电子邮件地址的其他信息。 在这种情况下，在用户第一次单击该链接并登录时，可能不会设置 **grantedTo** 属性，直到兑换邀请链接。

<!-- {"blockType": "example", truncated: true, "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->

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

<!-- {"blockType": "example", truncated: true,"@odata.type": "microsoft.graph.permission", "name": "permission-invite-redeemed" } -->

```json
{
  "id": "1",
  "roles": ["write"],
  "grantedTo": {
    "user": {
      "id": "5D33DD65C6932946",
      "displayName": "Robin Danielsen"
    }
  },
  "grantedToV2": {
    "user": {
      "id": "5D33DD65C6932946",
      "displayName": "Robin Danielsen"
    },
    "siteUser": {
      "id": "1",
      "displayName": "Robin Danielsen",
      "loginName": "Robin Danielsen"
    }
  },
  "invitation": {
    "email": "rd@contoso.com",
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
| [邀请人员][invite]                                  | `POST /drive/items/{item-id}/invite`
| [更新](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [删除](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [添加用户至共享链接](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`
| [撤销授权](../api/permission-revokegrants.md)   | `POST /drive/items/{item-id}/permissions/{id}/revokeGrants`

[createLink]: ../api/driveitem-createlink.md
[grant]: ../api/permission-grant.md
[IdentitySet]: identityset.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[shares API]: ../api/shares-get.md
[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md
[SharePointIdentitySet]: sharePointIdentitySet.md

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
