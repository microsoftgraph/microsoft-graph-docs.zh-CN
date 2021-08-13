---
author: JeremyKelley
ms.date: 09/10/2017
title: 权限
localization_priority: Priority
description: Permission 资源提供有关授予 DriveItem 资源共享权限的相关信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0d46c94d66339ad5329107e50a781d6f2f4e507d048707cced64dae35748e7da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126387"
---
# <a name="permission-resource-type"></a>Permission 资源类型

命名空间：microsoft.graph

**Permission** 资源提供为 [DriveItem](driveitem.md) 资源授予的共享权限的相关信息。

共享权限具有许多不同的形式。**权限** 资源通过资源上的 facet 表示这些不同的形式。

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

| 属性      | 类型                                      | 说明
|:--------------|:------------------------------------------|:-----------------
| id            | String                                    | 在项目的所有权限中，某个权限的唯一标识符。只读。
| grantedTo     | [IdentitySet](identityset.md)             | 对于用户类型权限，此权限的用户和应用程序的详细信息。只读。
| grantedToIdentities | Collection([IdentitySet](identityset.md)) | 对于链接类型权限，被授予权限的用户的详细信息。只读。
| 邀请    | [SharingInvitation][]                     | 此权限的全部关联共享邀请的详细信息。只读。
| inheritedFrom | [ItemReference](itemreference.md)         | 如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。
| link          | [SharingLink][]                           | 如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。
| roles         | Collection of String                      | 权限类型，例如 `read`。有关角色的完整列表，请参阅如下内容。只读。
| shareId       | String                                    | 可通过 [**shares** API](../api/shares-get.md) 访问此共享项目的唯一令牌。只读。
| expirationDateTime  | DateTimeOffset              | DateTimeOffset 的格式 yyyy-MM-ddTHH:mm:ssZ 表示权限的过期时间。 DateTime.MinValue 表示此权限没有设置过期时间。 可选。
| HasPassword         | 布尔值                     | 这表示是否为该权限设置了密码，它只在响应中显示。 可选、只读和仅限 OneDrive 个人版。

permission 资源使用 _Facet_ 说明此资源表示的权限种类。

具有 [**链接**] [SharingLink] facet 的权限表示在该项上创建的共享链接。共享链接包含一个唯一令牌，可以为具有上述链接的任何人提供对项目的访问权限。

具有 [**Invitation**][SharingInvitation] Facet 的权限表示通过邀请特定用户或组访问文件而添加的权限。

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

### <a name="roles-property-values"></a>角色属性值

| 值              | 说明                                                                        |
|:------------------|:-------------------------------------------------------------------------------|
| 阅读            | 提供读取项的元数据和内容的功能。            |
| 写入           | 提供读取并修改项的元数据和内容的功能。 |
| 所有者           | 对于 SharePoint 和 OneDrive for Business，这表示所有者角色。       |

## <a name="sharing-links"></a>共享链接
最常见的权限类型是共享链接。 共享链接提供唯一 URL，其中包含要共享的资源，以及提供对此资源的访问权限的身份验证令牌。 用户无需登录，即可访问通过共享链接共享的内容。 用户可以共享链接，从而提供对内容的只读权限或写入权限。

### <a name="view-link"></a>查看链接
查看链接提供对项的只读权限。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-view-link" } -->
```json
{
  "id": "1",
  "roles": ["read"],
  "link": {
    "type": "view",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
}
```

### <a name="edit-link"></a>编辑链接
编辑链接提供对项的读取和写入权限。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-edit-link" } -->
```json
{
  "id": "2",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
}
```
### <a name="specific-people-link"></a>特定人员链接

此链接向 `grantedToIdentities` 集合中的特定人员提供读写访问权限。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-people-link" } -->

```json
{
  "id": "3",
  "grantedToIdentities": [
    {
       "user": {
        "id": "35fij1974gb8832",
        "displayName&quot;: &quot;Misty Suarez"
      }
    },
    {
       "user": {
        "id": "9397721fh4hgh73",
        "displayName&quot;: &quot;Judith Clemons"
      }
    }
  ],
  "roles": ["write"],
  "link": {
    "webUrl": "https://contoso.sharepoint.com/:w:/t/design/a577ghg9hgh737613bmbjf839026561fmzhsr85ng9f3hjck2t5s",
    "application": { "id": "1234", "displayName": "Sample Application" }
  },
  "shareId": "!LKj1lkdlals90j1nlkascl",
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
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
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
}
```

### <a name="sharing-invitation"></a>共享邀请
除了创建共享链接之外，还可以通过电子邮件地址邀请用户。 在此方案中，权限创建的是发送到用户电子邮件地址的邀请。

#### <a name="invitation-to-an-email-address"></a>发送到电子邮件地址的邀请
如果权限是通过电子邮件地址发送给没有匹配帐户的接收者，那么在用户首次单击链接并登录以兑换邀请前，可能无法设置 **grantedTo** 属性。

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@gmail.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
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
      "displayName&quot;: &quot;John Doe"
    }
  },
  "invitation": {
    "email": "jd@outlook.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U",
  "expirationDateTime&quot;: &quot;0001-01-01T00:00:00Z"
}
```

## <a name="methods"></a>方法

| 方法                                                   | REST 路径
|:---------------------------------------------------------|:-----------------------
| [列出权限](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [获取权限](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [添加](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [更新](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [删除](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [添加用户至共享链接](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`


## <a name="remarks"></a>说明

OneDrive for Business 和 SharePoint 文档库不返回 **inheritedFrom** 属性。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->

