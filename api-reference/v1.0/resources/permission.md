---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Permission
localization_priority: Priority
ms.openlocfilehash: 988a4d6dcd1b04b34c5d2d03aca404b0a570922f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834165"
---
# <a name="permission-resource-type"></a><span data-ttu-id="e9eea-102">Permission 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9eea-102">Permission resource type</span></span>

<span data-ttu-id="e9eea-103">\*\*\*\* Permission 资源提供为 [DriveItem](driveitem.md) 资源授予的共享权限的相关信息。</span><span class="sxs-lookup"><span data-stu-id="e9eea-103">The **Permission** resource provides information about a sharing permission granted for a [DriveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="e9eea-104">共享权限具有许多不同的形式。</span><span class="sxs-lookup"><span data-stu-id="e9eea-104">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="e9eea-105">\*\*\*\* Permission 资源通过资源上的 facet 表示这些不同的形式。</span><span class="sxs-lookup"><span data-stu-id="e9eea-105">The **Permission** resource represents these different forms through facets on the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9eea-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9eea-106">JSON representation</span></span>

<span data-ttu-id="e9eea-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9eea-107">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "link",
    "grantedTo",
    "invitation",
    "inheritedFrom",
    "shareId"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.permission"
}-->
```json
{
  "id": "string (identifier)",
  "grantedTo": {"@odata.type": "microsoft.graph.identitySet"},
  "inheritedFrom": {"@odata.type": "microsoft.graph.itemReference"},
  "invitation": {"@odata.type": "microsoft.graph.sharingInvitation"},
  "link": {"@odata.type": "microsoft.graph.sharingLink"},
  "roles": ["string"],
  "shareId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="e9eea-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9eea-108">Properties</span></span>

| <span data-ttu-id="e9eea-109">属性</span><span class="sxs-lookup"><span data-stu-id="e9eea-109">Property</span></span>      | <span data-ttu-id="e9eea-110">类型</span><span class="sxs-lookup"><span data-stu-id="e9eea-110">Type</span></span>                                      | <span data-ttu-id="e9eea-111">说明</span><span class="sxs-lookup"><span data-stu-id="e9eea-111">Description</span></span>
|:--------------|:------------------------------------------|:-----------------
| <span data-ttu-id="e9eea-112">id</span><span class="sxs-lookup"><span data-stu-id="e9eea-112">id</span></span>            | <span data-ttu-id="e9eea-113">String</span><span class="sxs-lookup"><span data-stu-id="e9eea-113">String</span></span>                                    | <span data-ttu-id="e9eea-p102">在项目的所有权限中，某个权限的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e9eea-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="e9eea-116">grantedTo</span><span class="sxs-lookup"><span data-stu-id="e9eea-116">grantedTo</span></span>     | [<span data-ttu-id="e9eea-117">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e9eea-117">IdentitySet</span></span>](identityset.md)             | <span data-ttu-id="e9eea-p103">对于用户类型权限，此权限的用户和应用程序的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="e9eea-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="e9eea-120">邀请</span><span class="sxs-lookup"><span data-stu-id="e9eea-120">invitation</span></span>    | <span data-ttu-id="e9eea-121">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="e9eea-121">[SharingInvitation][]</span></span>                     | <span data-ttu-id="e9eea-p104">此权限的全部关联共享邀请的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="e9eea-p104">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="e9eea-124">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="e9eea-124">inheritedFrom</span></span> | [<span data-ttu-id="e9eea-125">ItemReference</span><span class="sxs-lookup"><span data-stu-id="e9eea-125">ItemReference</span></span>](itemreference.md)         | <span data-ttu-id="e9eea-p105">如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。</span><span class="sxs-lookup"><span data-stu-id="e9eea-p105">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="e9eea-128">link</span><span class="sxs-lookup"><span data-stu-id="e9eea-128">link</span></span>          | <span data-ttu-id="e9eea-129">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="e9eea-129">[SharingLink][]</span></span>                           | <span data-ttu-id="e9eea-p106">如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="e9eea-p106">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="e9eea-132">roles</span><span class="sxs-lookup"><span data-stu-id="e9eea-132">roles</span></span>         | <span data-ttu-id="e9eea-133">Collection of String</span><span class="sxs-lookup"><span data-stu-id="e9eea-133">Collection of String</span></span>                      | <span data-ttu-id="e9eea-p107">权限类型，例如 `read`。有关角色的完整列表，请参阅如下内容。只读。</span><span class="sxs-lookup"><span data-stu-id="e9eea-p107">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="e9eea-137">shareId</span><span class="sxs-lookup"><span data-stu-id="e9eea-137">shareId</span></span>       | <span data-ttu-id="e9eea-138">String</span><span class="sxs-lookup"><span data-stu-id="e9eea-138">String</span></span>                                    | <span data-ttu-id="e9eea-p108">可通过 [**shares** API](../api/shares-get.md) 访问此共享项目的唯一令牌。只读。</span><span class="sxs-lookup"><span data-stu-id="e9eea-p108">A unique token that can be used to access this shared item via the [**shares** API](../api/shares-get.md). Read-only.</span></span>

<span data-ttu-id="e9eea-141">permission 资源使用 _Facet_ 说明此资源表示的权限种类。</span><span class="sxs-lookup"><span data-stu-id="e9eea-141">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="e9eea-p109">具有[**链接**] [SharingLink] facet 的权限表示在该项上创建的共享链接。共享链接包含一个唯一令牌，可以为具有上述链接的任何人提供对项目的访问权限。</span><span class="sxs-lookup"><span data-stu-id="e9eea-p109">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="e9eea-144">具有 [**Invitation**][SharingInvitation] Facet 的权限表示通过邀请特定用户或组访问文件而添加的权限。</span><span class="sxs-lookup"><span data-stu-id="e9eea-144">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

## <a name="roles-enumeration"></a><span data-ttu-id="e9eea-147">角色枚举</span><span class="sxs-lookup"><span data-stu-id="e9eea-147">Roles enumeration</span></span>

| <span data-ttu-id="e9eea-148">角色</span><span class="sxs-lookup"><span data-stu-id="e9eea-148">Role</span></span>        | <span data-ttu-id="e9eea-149">详细信息</span><span class="sxs-lookup"><span data-stu-id="e9eea-149">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="e9eea-150">提供读取项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="e9eea-150">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="e9eea-151">提供读取并修改项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="e9eea-151">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="e9eea-152">对于 SharePoint 和 OneDrive for Business，这表示所有者角色。</span><span class="sxs-lookup"><span data-stu-id="e9eea-152">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="e9eea-153">对于 SharePoint 和 OneDrive for Business，这表示成员角色。</span><span class="sxs-lookup"><span data-stu-id="e9eea-153">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

## <a name="sharing-links"></a><span data-ttu-id="e9eea-154">共享链接</span><span class="sxs-lookup"><span data-stu-id="e9eea-154">Sharing links</span></span>
<span data-ttu-id="e9eea-155">最常见的权限类型是共享链接。</span><span class="sxs-lookup"><span data-stu-id="e9eea-155">The most common type of permissions are sharing links.</span></span>
<span data-ttu-id="e9eea-156">共享链接提供唯一 URL，其中包含要共享的资源，以及提供对此资源的访问权限的身份验证令牌。</span><span class="sxs-lookup"><span data-stu-id="e9eea-156">Sharing links provide a unique URL that includes both the resource being shared and an authentication token that provides access to the resource.</span></span> <span data-ttu-id="e9eea-157">用户无需登录，即可访问通过共享链接共享的内容。</span><span class="sxs-lookup"><span data-stu-id="e9eea-157">Users don't need to sign-in to access the content shared with a sharing link.</span></span> <span data-ttu-id="e9eea-158">用户可以共享链接，从而提供对内容的只读权限或写入权限。</span><span class="sxs-lookup"><span data-stu-id="e9eea-158">Users can share a link that gives read-only access to the content or writable access to the content.</span></span>

### <a name="view-link"></a><span data-ttu-id="e9eea-159">查看链接</span><span class="sxs-lookup"><span data-stu-id="e9eea-159">View Link</span></span>
<span data-ttu-id="e9eea-160">查看链接提供对项的只读权限。</span><span class="sxs-lookup"><span data-stu-id="e9eea-160">A view link provides read-only access to an item.</span></span>

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
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="edit-link"></a><span data-ttu-id="e9eea-161">编辑链接</span><span class="sxs-lookup"><span data-stu-id="e9eea-161">Edit link</span></span>
<span data-ttu-id="e9eea-162">编辑链接提供对项的读取和写入权限。</span><span class="sxs-lookup"><span data-stu-id="e9eea-162">An edit link provides read and write access to an item.</span></span>

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
  "shareId": "!LKj1lkdlals90j1nlkascl"
}
```

### <a name="sharing-invitation"></a><span data-ttu-id="e9eea-163">共享邀请</span><span class="sxs-lookup"><span data-stu-id="e9eea-163">Sharing Invitation</span></span>
<span data-ttu-id="e9eea-164">除了创建共享链接之外，还可以通过电子邮件地址邀请用户。</span><span class="sxs-lookup"><span data-stu-id="e9eea-164">In addition to creating sharing links, a user can be invited by e-mail address.</span></span>
<span data-ttu-id="e9eea-165">在此方案中，权限创建的是发送到用户电子邮件地址的邀请。</span><span class="sxs-lookup"><span data-stu-id="e9eea-165">In this scenario the permission creates an invitation that is sent to the user's email.</span></span>

#### <a name="invitation-to-an-email-address"></a><span data-ttu-id="e9eea-166">发送到电子邮件地址的邀请</span><span class="sxs-lookup"><span data-stu-id="e9eea-166">Invitation to an email address</span></span>
<span data-ttu-id="e9eea-167">如果权限是通过电子邮件地址发送给没有匹配帐户的接收者，那么在用户首次单击链接并登录以兑换邀请前，可能无法设置 **grantedTo** 属性。</span><span class="sxs-lookup"><span data-stu-id="e9eea-167">If the permission was sent via an email address to a recipient who does not have a matching account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time a user clicks the link and signs in.</span></span>

<!-- {"blockType": "example", "@odata.type": "microsoft.graph.permission", "name": "permission-invite-email" } -->
```json
{
  "id": "1",
  "roles": ["write"],
  "invitation": {
    "email": "jd@gmail.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
}
```

<span data-ttu-id="e9eea-168">在用户兑换共享邀请后，**grantedTo** 属性将包含兑换权限的帐户的相关信息：</span><span class="sxs-lookup"><span data-stu-id="e9eea-168">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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
    "email": "jd@outlook.com",
    "signInRequired": true
  },
  "shareId": "FWxc1lasfdbEAGM5fI7B67aB5ZMPDMmQ11U"
}
```

## <a name="methods"></a><span data-ttu-id="e9eea-169">方法</span><span class="sxs-lookup"><span data-stu-id="e9eea-169">Methods</span></span>

| <span data-ttu-id="e9eea-170">方法</span><span class="sxs-lookup"><span data-stu-id="e9eea-170">Method</span></span>                                                   | <span data-ttu-id="e9eea-171">REST 路径</span><span class="sxs-lookup"><span data-stu-id="e9eea-171">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="e9eea-172">列出权限</span><span class="sxs-lookup"><span data-stu-id="e9eea-172">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="e9eea-173">获取权限</span><span class="sxs-lookup"><span data-stu-id="e9eea-173">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="e9eea-174">添加</span><span class="sxs-lookup"><span data-stu-id="e9eea-174">Add</span></span>](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="e9eea-175">更新</span><span class="sxs-lookup"><span data-stu-id="e9eea-175">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="e9eea-176">删除</span><span class="sxs-lookup"><span data-stu-id="e9eea-176">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`


## <a name="remarks"></a><span data-ttu-id="e9eea-177">注解</span><span class="sxs-lookup"><span data-stu-id="e9eea-177">Remarks</span></span>

<span data-ttu-id="e9eea-178">OneDrive for Business 和 SharePoint 文档库不返回 **inheritedFrom** 属性。</span><span class="sxs-lookup"><span data-stu-id="e9eea-178">OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
