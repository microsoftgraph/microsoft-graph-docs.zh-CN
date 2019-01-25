---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permission
localization_priority: Normal
ms.openlocfilehash: 6a5a0af9c95900232ff87aa7aedb731a83a91cc5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518847"
---
# <a name="permission-resource-type"></a><span data-ttu-id="50e72-102">Permission 资源类型</span><span class="sxs-lookup"><span data-stu-id="50e72-102">permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50e72-103">\*\*\*\* Permission 资源提供为 [DriveItem](driveitem.md) 资源授予的共享权限的相关信息。</span><span class="sxs-lookup"><span data-stu-id="50e72-103">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="50e72-104">共享权限具有许多不同的形式。</span><span class="sxs-lookup"><span data-stu-id="50e72-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="50e72-105">\*\*\*\* Permission 资源通过资源上的 facet 表示这些不同的形式。</span><span class="sxs-lookup"><span data-stu-id="50e72-105">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="50e72-106">**注意：** OneDrive for Business 和 SharePoint 文档库不返回**inheritedFrom**属性。</span><span class="sxs-lookup"><span data-stu-id="50e72-106">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50e72-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50e72-107">JSON representation</span></span>

<span data-ttu-id="50e72-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50e72-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="50e72-109">属性</span><span class="sxs-lookup"><span data-stu-id="50e72-109">Properties</span></span>

| <span data-ttu-id="50e72-110">属性</span><span class="sxs-lookup"><span data-stu-id="50e72-110">Property</span></span>            | <span data-ttu-id="50e72-111">类型</span><span class="sxs-lookup"><span data-stu-id="50e72-111">Type</span></span>                        | <span data-ttu-id="50e72-112">说明</span><span class="sxs-lookup"><span data-stu-id="50e72-112">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="50e72-113">id</span><span class="sxs-lookup"><span data-stu-id="50e72-113">id</span></span>                  | <span data-ttu-id="50e72-114">String</span><span class="sxs-lookup"><span data-stu-id="50e72-114">String</span></span>                      | <span data-ttu-id="50e72-p102">在项目的所有权限中，某个权限的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="50e72-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="50e72-117">grantedTo</span><span class="sxs-lookup"><span data-stu-id="50e72-117">grantedTo</span></span>           | <span data-ttu-id="50e72-118">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="50e72-118">[IdentitySet][]</span></span>             | <span data-ttu-id="50e72-p103">对于用户类型权限，此权限的用户和应用程序的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="50e72-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="50e72-121">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="50e72-121">grantedToIdentities</span></span> | <span data-ttu-id="50e72-122">集合 ([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="50e72-122">Collection([IdentitySet][])</span></span> | <span data-ttu-id="50e72-123">有关链接类型的权限，向其授予权限的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="50e72-123">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="50e72-124">只读。</span><span class="sxs-lookup"><span data-stu-id="50e72-124">Read-only.</span></span>
| <span data-ttu-id="50e72-125">邀请</span><span class="sxs-lookup"><span data-stu-id="50e72-125">invitation</span></span>          | <span data-ttu-id="50e72-126">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="50e72-126">[SharingInvitation][]</span></span>       | <span data-ttu-id="50e72-p105">此权限的全部关联共享邀请的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="50e72-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="50e72-129">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="50e72-129">inheritedFrom</span></span>       | <span data-ttu-id="50e72-130">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="50e72-130">[ItemReference][]</span></span>           | <span data-ttu-id="50e72-p106">如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。</span><span class="sxs-lookup"><span data-stu-id="50e72-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="50e72-133">link</span><span class="sxs-lookup"><span data-stu-id="50e72-133">link</span></span>                | <span data-ttu-id="50e72-134">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="50e72-134">[SharingLink][]</span></span>             | <span data-ttu-id="50e72-p107">如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="50e72-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="50e72-137">roles</span><span class="sxs-lookup"><span data-stu-id="50e72-137">roles</span></span>               | <span data-ttu-id="50e72-138">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="50e72-138">Collection(String)</span></span>          | <span data-ttu-id="50e72-p108">权限类型，例如 `read`。有关角色的完整列表，请参阅如下内容。只读。</span><span class="sxs-lookup"><span data-stu-id="50e72-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="50e72-142">shareId</span><span class="sxs-lookup"><span data-stu-id="50e72-142">shareId</span></span>             | <span data-ttu-id="50e72-143">String</span><span class="sxs-lookup"><span data-stu-id="50e72-143">String</span></span>                      | <span data-ttu-id="50e72-p109">可通过 **[shares][] API** 访问此共享项目的唯一令牌。只读。</span><span class="sxs-lookup"><span data-stu-id="50e72-p109">A unique token that can be used to access this shared item via the **[shares API][]**. Read-only.</span></span>
| <span data-ttu-id="50e72-146">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="50e72-146">expirationDateTime</span></span>  | <span data-ttu-id="50e72-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50e72-147">DateTimeOffset</span></span>              | <span data-ttu-id="50e72-148">一种格式的 yyyy-MM-ddTHH:mm:ssZ 方法的指示权限的到期时间。</span><span class="sxs-lookup"><span data-stu-id="50e72-148">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="50e72-149">DateTime.MinValue 表示那里无过期期限设置此权限。</span><span class="sxs-lookup"><span data-stu-id="50e72-149">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="50e72-150">可选。</span><span class="sxs-lookup"><span data-stu-id="50e72-150">Optional.</span></span>
| <span data-ttu-id="50e72-151">HasPassword</span><span class="sxs-lookup"><span data-stu-id="50e72-151">hasPassword</span></span>         | <span data-ttu-id="50e72-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="50e72-152">Boolean</span></span>                     | <span data-ttu-id="50e72-153">这指示是否将密码设置此权限，仅显示响应。</span><span class="sxs-lookup"><span data-stu-id="50e72-153">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="50e72-154">可选只读和仅 OneDrive 个人。</span><span class="sxs-lookup"><span data-stu-id="50e72-154">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="50e72-155">角色枚举值</span><span class="sxs-lookup"><span data-stu-id="50e72-155">Roles enumeration values</span></span>

| <span data-ttu-id="50e72-156">值</span><span class="sxs-lookup"><span data-stu-id="50e72-156">Value</span></span>        | <span data-ttu-id="50e72-157">详细信息</span><span class="sxs-lookup"><span data-stu-id="50e72-157">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="50e72-158">提供读取项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="50e72-158">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="50e72-159">提供读取并修改项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="50e72-159">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="50e72-160">对于 SharePoint 和 OneDrive for Business，这表示所有者角色。</span><span class="sxs-lookup"><span data-stu-id="50e72-160">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="50e72-161">对于 SharePoint 和 OneDrive for Business，这表示成员角色。</span><span class="sxs-lookup"><span data-stu-id="50e72-161">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="50e72-162">permission 资源使用 _Facet_ 说明此资源表示的权限种类。</span><span class="sxs-lookup"><span data-stu-id="50e72-162">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="50e72-163">共享链接包含一个唯一的标记所需访问的项目。</span><span class="sxs-lookup"><span data-stu-id="50e72-163">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="50e72-164">具有 [**Invitation**][SharingInvitation] Facet 的权限表示通过邀请特定用户或组访问文件而添加的权限。</span><span class="sxs-lookup"><span data-stu-id="50e72-164">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="50e72-165">共享链接</span><span class="sxs-lookup"><span data-stu-id="50e72-165">Sharing links</span></span>

<span data-ttu-id="50e72-166">使用共享对项目创建链接的[**链接**][SharingLink]方面表示的权限。</span><span class="sxs-lookup"><span data-stu-id="50e72-166">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="50e72-167">这些是最常见类型的权限。</span><span class="sxs-lookup"><span data-stu-id="50e72-167">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="50e72-168">共享链接提供了一个可用于访问文件或文件夹的唯一的 URL。</span><span class="sxs-lookup"><span data-stu-id="50e72-168">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="50e72-169">他们可以设置授予多种方式访问权限。</span><span class="sxs-lookup"><span data-stu-id="50e72-169">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="50e72-170">例如，您可以使用[createLink][] API 创建链接的适用于任何人登录到您的组织，或您可以创建适用于任何人，而无需登录的链接。</span><span class="sxs-lookup"><span data-stu-id="50e72-170">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="50e72-171">可以使用[邀请][]API，无论他们是在您的公司或未创建仅适用于特定用户的链接。</span><span class="sxs-lookup"><span data-stu-id="50e72-171">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="50e72-172">下面是共享链接的一些示例。</span><span class="sxs-lookup"><span data-stu-id="50e72-172">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="50e72-173">查看链接</span><span class="sxs-lookup"><span data-stu-id="50e72-173">View link</span></span>

<span data-ttu-id="50e72-174">此视图链接与链接的任何人都提供只读访问权限。</span><span class="sxs-lookup"><span data-stu-id="50e72-174">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="50e72-175">编辑链接</span><span class="sxs-lookup"><span data-stu-id="50e72-175">Edit link</span></span>

<span data-ttu-id="50e72-176">此编辑链接与链接组织中的任何人都提供读取和写入访问。</span><span class="sxs-lookup"><span data-stu-id="50e72-176">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="50e72-177">特定人员链接</span><span class="sxs-lookup"><span data-stu-id="50e72-177">Specific people link</span></span>

<span data-ttu-id="50e72-178">此链接提供读取和写入访问中的特定人员`grantedToIdentities`集合。</span><span class="sxs-lookup"><span data-stu-id="50e72-178">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="50e72-179">共享邀请</span><span class="sxs-lookup"><span data-stu-id="50e72-179">Sharing invitations</span></span>

<span data-ttu-id="50e72-180">发送的[邀请][]API 的权限可能具有[邀请][SharingInvitation]方面中的其他信息。</span><span class="sxs-lookup"><span data-stu-id="50e72-180">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="50e72-181">如果邀请发送给不匹配的已知的帐户的电子邮件地址， **grantedTo**属性可能不设置直到邀请会兑换，其中第一次用户单击的链接并登录时，发生此事件。</span><span class="sxs-lookup"><span data-stu-id="50e72-181">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="50e72-182">在用户兑换共享邀请后，**grantedTo** 属性将包含兑换权限的帐户的相关信息：</span><span class="sxs-lookup"><span data-stu-id="50e72-182">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="50e72-183">方法</span><span class="sxs-lookup"><span data-stu-id="50e72-183">Methods</span></span>

| <span data-ttu-id="50e72-184">方法</span><span class="sxs-lookup"><span data-stu-id="50e72-184">Method</span></span>                                                   | <span data-ttu-id="50e72-185">REST 路径</span><span class="sxs-lookup"><span data-stu-id="50e72-185">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="50e72-186">列出权限</span><span class="sxs-lookup"><span data-stu-id="50e72-186">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="50e72-187">获取权限</span><span class="sxs-lookup"><span data-stu-id="50e72-187">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="50e72-188">[创建链接][createLink]</span><span class="sxs-lookup"><span data-stu-id="50e72-188">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="50e72-189">[邀请其他人][邀请]</span><span class="sxs-lookup"><span data-stu-id="50e72-189">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="50e72-190">更新</span><span class="sxs-lookup"><span data-stu-id="50e72-190">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="50e72-191">删除</span><span class="sxs-lookup"><span data-stu-id="50e72-191">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



[createLink]: ../api/driveitem-createlink.md
[IdentitySet]: identityset.md
[邀请]: ../api/driveitem-invite.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
[共享 API]: ../api/shares-get.md
[shares API]: ../api/shares-get.md
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
  "suppressions": [
    "Error: /api-reference/beta/resources/permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
