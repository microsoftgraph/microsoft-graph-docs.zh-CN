---
author: JeremyKelley
ms.date: 09/10/2017
title: 权限
localization_priority: Priority
description: Permission 资源提供有关授予 DriveItem 资源共享权限的相关信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5c14371966d4620450c7d791a3ed90a38b12c61b
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335604"
---
# <a name="permission-resource-type"></a><span data-ttu-id="da744-103">Permission 资源类型</span><span class="sxs-lookup"><span data-stu-id="da744-103">Permission resource type</span></span>

<span data-ttu-id="da744-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da744-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da744-105">**Permission** 资源提供为 [DriveItem](driveitem.md) 资源授予的共享权限的相关信息。</span><span class="sxs-lookup"><span data-stu-id="da744-105">The **Permission** resource provides information about a sharing permission granted for a [DriveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="da744-106">共享权限具有许多不同的形式。</span><span class="sxs-lookup"><span data-stu-id="da744-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="da744-107">**Permission** 资源通过资源上的 facet 表示这些不同的形式。</span><span class="sxs-lookup"><span data-stu-id="da744-107">The **Permission** resource represents these different forms through facets on the resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da744-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da744-108">JSON representation</span></span>

<span data-ttu-id="da744-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da744-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="da744-110">属性</span><span class="sxs-lookup"><span data-stu-id="da744-110">Properties</span></span>

| <span data-ttu-id="da744-111">属性</span><span class="sxs-lookup"><span data-stu-id="da744-111">Property</span></span>      | <span data-ttu-id="da744-112">类型</span><span class="sxs-lookup"><span data-stu-id="da744-112">Type</span></span>                                      | <span data-ttu-id="da744-113">说明</span><span class="sxs-lookup"><span data-stu-id="da744-113">Description</span></span>
|:--------------|:------------------------------------------|:-----------------
| <span data-ttu-id="da744-114">id</span><span class="sxs-lookup"><span data-stu-id="da744-114">id</span></span>            | <span data-ttu-id="da744-115">String</span><span class="sxs-lookup"><span data-stu-id="da744-115">String</span></span>                                    | <span data-ttu-id="da744-p102">在项目的所有权限中，某个权限的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="da744-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="da744-118">grantedTo</span><span class="sxs-lookup"><span data-stu-id="da744-118">grantedTo</span></span>     | [<span data-ttu-id="da744-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="da744-119">IdentitySet</span></span>](identityset.md)             | <span data-ttu-id="da744-p103">对于用户类型权限，此权限的用户和应用程序的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="da744-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="da744-122">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="da744-122">grantedToIdentities</span></span> | <span data-ttu-id="da744-123">Collection([IdentitySet](identityset.md))</span><span class="sxs-lookup"><span data-stu-id="da744-123">Collection([IdentitySet](identityset.md))</span></span> | <span data-ttu-id="da744-p104">对于链接类型权限，被授予权限的用户的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="da744-p104">For link type permissions, the details of the users to whom permission was granted. Read-only.</span></span>
| <span data-ttu-id="da744-126">邀请</span><span class="sxs-lookup"><span data-stu-id="da744-126">invitation</span></span>    | <span data-ttu-id="da744-127">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="da744-127">[SharingInvitation][]</span></span>                     | <span data-ttu-id="da744-p105">此权限的全部关联共享邀请的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="da744-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="da744-130">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="da744-130">inheritedFrom</span></span> | [<span data-ttu-id="da744-131">ItemReference</span><span class="sxs-lookup"><span data-stu-id="da744-131">ItemReference</span></span>](itemreference.md)         | <span data-ttu-id="da744-p106">如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。</span><span class="sxs-lookup"><span data-stu-id="da744-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="da744-134">link</span><span class="sxs-lookup"><span data-stu-id="da744-134">link</span></span>          | <span data-ttu-id="da744-135">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="da744-135">[SharingLink][]</span></span>                           | <span data-ttu-id="da744-p107">如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="da744-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="da744-138">roles</span><span class="sxs-lookup"><span data-stu-id="da744-138">roles</span></span>         | <span data-ttu-id="da744-139">Collection of String</span><span class="sxs-lookup"><span data-stu-id="da744-139">Collection of String</span></span>                      | <span data-ttu-id="da744-p108">权限类型，例如 `read`。有关角色的完整列表，请参阅如下内容。只读。</span><span class="sxs-lookup"><span data-stu-id="da744-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="da744-143">shareId</span><span class="sxs-lookup"><span data-stu-id="da744-143">shareId</span></span>       | <span data-ttu-id="da744-144">String</span><span class="sxs-lookup"><span data-stu-id="da744-144">String</span></span>                                    | <span data-ttu-id="da744-p109">可通过 [**shares** API](../api/shares-get.md) 访问此共享项目的唯一令牌。只读。</span><span class="sxs-lookup"><span data-stu-id="da744-p109">A unique token that can be used to access this shared item via the [**shares** API](../api/shares-get.md). Read-only.</span></span>
| <span data-ttu-id="da744-147">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="da744-147">expirationDateTime</span></span>  | <span data-ttu-id="da744-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da744-148">DateTimeOffset</span></span>              | <span data-ttu-id="da744-149">DateTimeOffset 的格式 yyyy-MM-ddTHH:mm:ssZ 表示权限的过期时间。</span><span class="sxs-lookup"><span data-stu-id="da744-149">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="da744-150">DateTime.MinValue 表示此权限没有设置过期时间。</span><span class="sxs-lookup"><span data-stu-id="da744-150">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="da744-151">可选。</span><span class="sxs-lookup"><span data-stu-id="da744-151">Optional.</span></span>
| <span data-ttu-id="da744-152">HasPassword</span><span class="sxs-lookup"><span data-stu-id="da744-152">hasPassword</span></span>         | <span data-ttu-id="da744-153">布尔值</span><span class="sxs-lookup"><span data-stu-id="da744-153">Boolean</span></span>                     | <span data-ttu-id="da744-154">这表示是否为该权限设置了密码，它只在响应中显示。</span><span class="sxs-lookup"><span data-stu-id="da744-154">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="da744-155">可选、只读和仅限 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="da744-155">Optional and Read-only and for OneDrive Personal only.</span></span>

<span data-ttu-id="da744-156">permission 资源使用 _Facet_ 说明此资源表示的权限种类。</span><span class="sxs-lookup"><span data-stu-id="da744-156">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="da744-p112">具有 [**链接**] [SharingLink] facet 的权限表示在该项上创建的共享链接。共享链接包含一个唯一令牌，可以为具有上述链接的任何人提供对项目的访问权限。</span><span class="sxs-lookup"><span data-stu-id="da744-p112">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="da744-159">具有 [**Invitation**][SharingInvitation] Facet 的权限表示通过邀请特定用户或组访问文件而添加的权限。</span><span class="sxs-lookup"><span data-stu-id="da744-159">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

[SharingInvitation]: sharinginvitation.md
[SharingLink]: sharinglink.md

### <a name="roles-property-values"></a><span data-ttu-id="da744-162">角色属性值</span><span class="sxs-lookup"><span data-stu-id="da744-162">Roles property values</span></span>

| <span data-ttu-id="da744-163">值</span><span class="sxs-lookup"><span data-stu-id="da744-163">Value</span></span>              | <span data-ttu-id="da744-164">说明</span><span class="sxs-lookup"><span data-stu-id="da744-164">Description</span></span>                                                                        |
|:------------------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="da744-165">阅读</span><span class="sxs-lookup"><span data-stu-id="da744-165">read</span></span>            | <span data-ttu-id="da744-166">提供读取项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="da744-166">Provides the ability to read the metadata and contents of the item.</span></span>            |
| <span data-ttu-id="da744-167">写入</span><span class="sxs-lookup"><span data-stu-id="da744-167">write</span></span>           | <span data-ttu-id="da744-168">提供读取并修改项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="da744-168">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| <span data-ttu-id="da744-169">所有者</span><span class="sxs-lookup"><span data-stu-id="da744-169">owner</span></span>           | <span data-ttu-id="da744-170">对于 SharePoint 和 OneDrive for Business，这表示所有者角色。</span><span class="sxs-lookup"><span data-stu-id="da744-170">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |

## <a name="sharing-links"></a><span data-ttu-id="da744-171">共享链接</span><span class="sxs-lookup"><span data-stu-id="da744-171">Sharing links</span></span>
<span data-ttu-id="da744-p113">最常见的权限类型是共享链接。 共享链接提供唯一 URL，其中包含要共享的资源，以及提供对此资源的访问权限的身份验证令牌。 用户无需登录，即可访问通过共享链接共享的内容。 用户可以共享链接，从而提供对内容的只读权限或写入权限。</span><span class="sxs-lookup"><span data-stu-id="da744-p113">The most common type of permissions are sharing links. Sharing links provide a unique URL that includes both the resource being shared and an authentication token that provides access to the resource. Users don't need to sign-in to access the content shared with a sharing link. Users can share a link that gives read-only access to the content or writable access to the content.</span></span>

### <a name="view-link"></a><span data-ttu-id="da744-176">查看链接</span><span class="sxs-lookup"><span data-stu-id="da744-176">View Link</span></span>
<span data-ttu-id="da744-177">查看链接提供对项的只读权限。</span><span class="sxs-lookup"><span data-stu-id="da744-177">A view link provides read-only access to an item.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="da744-178">编辑链接</span><span class="sxs-lookup"><span data-stu-id="da744-178">Edit link</span></span>
<span data-ttu-id="da744-179">编辑链接提供对项的读取和写入权限。</span><span class="sxs-lookup"><span data-stu-id="da744-179">An edit link provides read and write access to an item.</span></span>

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
### <a name="specific-people-link"></a><span data-ttu-id="da744-180">特定人员链接</span><span class="sxs-lookup"><span data-stu-id="da744-180">Specific people link</span></span>

<span data-ttu-id="da744-181">此链接向 `grantedToIdentities` 集合中的特定人员提供读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="da744-181">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

### <a name="existing-access-link"></a><span data-ttu-id="da744-182">现有的访问链接</span><span class="sxs-lookup"><span data-stu-id="da744-182">Existing access link</span></span>

<span data-ttu-id="da744-183">此链接不会向用户授予任何其他特权。</span><span class="sxs-lookup"><span data-stu-id="da744-183">This link does not grant any additional privileges to the user.</span></span>

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

### <a name="sharing-invitation"></a><span data-ttu-id="da744-184">共享邀请</span><span class="sxs-lookup"><span data-stu-id="da744-184">Sharing Invitation</span></span>
<span data-ttu-id="da744-p114">除了创建共享链接之外，还可以通过电子邮件地址邀请用户。 在此方案中，权限创建的是发送到用户电子邮件地址的邀请。</span><span class="sxs-lookup"><span data-stu-id="da744-p114">In addition to creating sharing links, a user can be invited by e-mail address. In this scenario the permission creates an invitation that is sent to the user's email.</span></span>

#### <a name="invitation-to-an-email-address"></a><span data-ttu-id="da744-187">发送到电子邮件地址的邀请</span><span class="sxs-lookup"><span data-stu-id="da744-187">Invitation to an email address</span></span>
<span data-ttu-id="da744-188">如果权限是通过电子邮件地址发送给没有匹配帐户的接收者，那么在用户首次单击链接并登录以兑换邀请前，可能无法设置 **grantedTo** 属性。</span><span class="sxs-lookup"><span data-stu-id="da744-188">If the permission was sent via an email address to a recipient who does not have a matching account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time a user clicks the link and signs in.</span></span>

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

<span data-ttu-id="da744-189">在用户兑换共享邀请后，**grantedTo** 属性将包含兑换权限的帐户的相关信息：</span><span class="sxs-lookup"><span data-stu-id="da744-189">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="da744-190">方法</span><span class="sxs-lookup"><span data-stu-id="da744-190">Methods</span></span>

| <span data-ttu-id="da744-191">方法</span><span class="sxs-lookup"><span data-stu-id="da744-191">Method</span></span>                                                   | <span data-ttu-id="da744-192">REST 路径</span><span class="sxs-lookup"><span data-stu-id="da744-192">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="da744-193">列出权限</span><span class="sxs-lookup"><span data-stu-id="da744-193">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="da744-194">获取权限</span><span class="sxs-lookup"><span data-stu-id="da744-194">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="da744-195">添加</span><span class="sxs-lookup"><span data-stu-id="da744-195">Add</span></span>](../api/driveitem-invite.md)                        | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="da744-196">更新</span><span class="sxs-lookup"><span data-stu-id="da744-196">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="da744-197">删除</span><span class="sxs-lookup"><span data-stu-id="da744-197">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="da744-198">添加用户至共享链接</span><span class="sxs-lookup"><span data-stu-id="da744-198">Add users to sharing link</span></span>](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`


## <a name="remarks"></a><span data-ttu-id="da744-199">说明</span><span class="sxs-lookup"><span data-stu-id="da744-199">Remarks</span></span>

<span data-ttu-id="da744-200">OneDrive for Business 和 SharePoint 文档库不返回 **inheritedFrom** 属性。</span><span class="sxs-lookup"><span data-stu-id="da744-200">OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->

