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
# <a name="permission-resource-type"></a><span data-ttu-id="019eb-102">权限资源类型</span><span class="sxs-lookup"><span data-stu-id="019eb-102">permission resource type</span></span>

> <span data-ttu-id="019eb-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="019eb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="019eb-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="019eb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="019eb-105">**权限**资源提供有关[driveItem](driveitem.md)资源授予共享权限的信息。</span><span class="sxs-lookup"><span data-stu-id="019eb-105">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="019eb-106">共享权限具有许多不同的形式。</span><span class="sxs-lookup"><span data-stu-id="019eb-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="019eb-107">**权限**资源表示这些不同的窗体，通过对资源的方面。</span><span class="sxs-lookup"><span data-stu-id="019eb-107">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="019eb-108">**注意：** OneDrive for Business 和 SharePoint 文档库不返回**inheritedFrom**属性。</span><span class="sxs-lookup"><span data-stu-id="019eb-108">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="019eb-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="019eb-109">JSON representation</span></span>

<span data-ttu-id="019eb-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="019eb-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="019eb-111">属性</span><span class="sxs-lookup"><span data-stu-id="019eb-111">Properties</span></span>

| <span data-ttu-id="019eb-112">属性</span><span class="sxs-lookup"><span data-stu-id="019eb-112">Property</span></span>            | <span data-ttu-id="019eb-113">类型</span><span class="sxs-lookup"><span data-stu-id="019eb-113">Type</span></span>                        | <span data-ttu-id="019eb-114">说明</span><span class="sxs-lookup"><span data-stu-id="019eb-114">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="019eb-115">id</span><span class="sxs-lookup"><span data-stu-id="019eb-115">id</span></span>                  | <span data-ttu-id="019eb-116">字符串</span><span class="sxs-lookup"><span data-stu-id="019eb-116">String</span></span>                      | <span data-ttu-id="019eb-p103">在项目的所有权限中，某个权限的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="019eb-p103">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="019eb-119">grantedTo</span><span class="sxs-lookup"><span data-stu-id="019eb-119">grantedTo</span></span>           | <span data-ttu-id="019eb-120">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="019eb-120">[IdentitySet][]</span></span>             | <span data-ttu-id="019eb-p104">对于用户类型权限，此权限的用户和应用程序的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="019eb-p104">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="019eb-123">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="019eb-123">grantedToIdentities</span></span> | <span data-ttu-id="019eb-124">集合 ([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="019eb-124">Collection([IdentitySet][])</span></span> | <span data-ttu-id="019eb-125">有关链接类型的权限，向其授予权限的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="019eb-125">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="019eb-126">只读。</span><span class="sxs-lookup"><span data-stu-id="019eb-126">Read-only.</span></span>
| <span data-ttu-id="019eb-127">邀请</span><span class="sxs-lookup"><span data-stu-id="019eb-127">invitation</span></span>          | <span data-ttu-id="019eb-128">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="019eb-128">[SharingInvitation][]</span></span>       | <span data-ttu-id="019eb-p106">此权限的全部关联共享邀请的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="019eb-p106">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="019eb-131">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="019eb-131">inheritedFrom</span></span>       | <span data-ttu-id="019eb-132">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="019eb-132">[ItemReference][]</span></span>           | <span data-ttu-id="019eb-p107">如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。</span><span class="sxs-lookup"><span data-stu-id="019eb-p107">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="019eb-135">link</span><span class="sxs-lookup"><span data-stu-id="019eb-135">link</span></span>                | <span data-ttu-id="019eb-136">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="019eb-136">[SharingLink][]</span></span>             | <span data-ttu-id="019eb-p108">如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="019eb-p108">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="019eb-139">roles</span><span class="sxs-lookup"><span data-stu-id="019eb-139">roles</span></span>               | <span data-ttu-id="019eb-140">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="019eb-140">Collection(String)</span></span>          | <span data-ttu-id="019eb-p109">权限类型，例如 `read`。有关角色的完整列表，请参阅如下内容。只读。</span><span class="sxs-lookup"><span data-stu-id="019eb-p109">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="019eb-144">shareId</span><span class="sxs-lookup"><span data-stu-id="019eb-144">shareId</span></span>             | <span data-ttu-id="019eb-145">字符串</span><span class="sxs-lookup"><span data-stu-id="019eb-145">String</span></span>                      | <span data-ttu-id="019eb-146">一个可用于访问此**[共享 API][]** 通过共享项目的唯一标记。</span><span class="sxs-lookup"><span data-stu-id="019eb-146">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="019eb-147">只读。</span><span class="sxs-lookup"><span data-stu-id="019eb-147">Read-only.</span></span>
| <span data-ttu-id="019eb-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="019eb-148">expirationDateTime</span></span>  | <span data-ttu-id="019eb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="019eb-149">DateTimeOffset</span></span>              | <span data-ttu-id="019eb-150">一种格式的 yyyy-MM-ddTHH:mm:ssZ 方法的指示权限的到期时间。</span><span class="sxs-lookup"><span data-stu-id="019eb-150">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="019eb-151">DateTime.MinValue 表示那里无过期期限设置此权限。</span><span class="sxs-lookup"><span data-stu-id="019eb-151">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="019eb-152">可选。</span><span class="sxs-lookup"><span data-stu-id="019eb-152">Optional.</span></span>
| <span data-ttu-id="019eb-153">hasPassword</span><span class="sxs-lookup"><span data-stu-id="019eb-153">hasPassword</span></span>         | <span data-ttu-id="019eb-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="019eb-154">Boolean</span></span>                     | <span data-ttu-id="019eb-155">这指示是否将密码设置此权限，仅显示响应。</span><span class="sxs-lookup"><span data-stu-id="019eb-155">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="019eb-156">可选只读和仅 OneDrive 个人。</span><span class="sxs-lookup"><span data-stu-id="019eb-156">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="019eb-157">角色枚举值</span><span class="sxs-lookup"><span data-stu-id="019eb-157">Roles enumeration values</span></span>

| <span data-ttu-id="019eb-158">值</span><span class="sxs-lookup"><span data-stu-id="019eb-158">Value</span></span>        | <span data-ttu-id="019eb-159">详细信息</span><span class="sxs-lookup"><span data-stu-id="019eb-159">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="019eb-160">提供读取项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="019eb-160">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="019eb-161">提供读取并修改项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="019eb-161">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="019eb-162">对于 SharePoint 和 OneDrive for Business，这表示所有者角色。</span><span class="sxs-lookup"><span data-stu-id="019eb-162">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="019eb-163">对于 SharePoint 和 OneDrive for Business，这表示成员角色。</span><span class="sxs-lookup"><span data-stu-id="019eb-163">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="019eb-164">permission 资源使用 _Facet_ 说明此资源表示的权限种类。</span><span class="sxs-lookup"><span data-stu-id="019eb-164">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="019eb-165">共享链接包含一个唯一的标记所需访问的项目。</span><span class="sxs-lookup"><span data-stu-id="019eb-165">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="019eb-166">具有 [**Invitation**][SharingInvitation] Facet 的权限表示通过邀请特定用户或组访问文件而添加的权限。</span><span class="sxs-lookup"><span data-stu-id="019eb-166">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="019eb-167">共享链接</span><span class="sxs-lookup"><span data-stu-id="019eb-167">Sharing links</span></span>

<span data-ttu-id="019eb-168">使用共享对项目创建链接的[**链接**][SharingLink]方面表示的权限。</span><span class="sxs-lookup"><span data-stu-id="019eb-168">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="019eb-169">这些是最常见类型的权限。</span><span class="sxs-lookup"><span data-stu-id="019eb-169">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="019eb-170">共享链接提供了一个可用于访问文件或文件夹的唯一的 URL。</span><span class="sxs-lookup"><span data-stu-id="019eb-170">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="019eb-171">他们可以设置授予多种方式访问权限。</span><span class="sxs-lookup"><span data-stu-id="019eb-171">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="019eb-172">例如，您可以使用[createLink][] API 创建链接的适用于任何人登录到您的组织，或您可以创建适用于任何人，而无需登录的链接。</span><span class="sxs-lookup"><span data-stu-id="019eb-172">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="019eb-173">可以使用[邀请][]API，无论他们是在您的公司或未创建仅适用于特定用户的链接。</span><span class="sxs-lookup"><span data-stu-id="019eb-173">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="019eb-174">下面是共享链接的一些示例。</span><span class="sxs-lookup"><span data-stu-id="019eb-174">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="019eb-175">查看链接</span><span class="sxs-lookup"><span data-stu-id="019eb-175">View link</span></span>

<span data-ttu-id="019eb-176">此视图链接与链接的任何人都提供只读访问权限。</span><span class="sxs-lookup"><span data-stu-id="019eb-176">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="019eb-177">编辑链接</span><span class="sxs-lookup"><span data-stu-id="019eb-177">Edit link</span></span>

<span data-ttu-id="019eb-178">此编辑链接与链接组织中的任何人都提供读取和写入访问。</span><span class="sxs-lookup"><span data-stu-id="019eb-178">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="019eb-179">特定人员链接</span><span class="sxs-lookup"><span data-stu-id="019eb-179">Specific people link</span></span>

<span data-ttu-id="019eb-180">此链接提供读取和写入访问中的特定人员`grantedToIdentities`集合。</span><span class="sxs-lookup"><span data-stu-id="019eb-180">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="019eb-181">共享邀请</span><span class="sxs-lookup"><span data-stu-id="019eb-181">Sharing invitations</span></span>

<span data-ttu-id="019eb-182">发送的[邀请][]API 的权限可能具有[邀请][SharingInvitation]方面中的其他信息。</span><span class="sxs-lookup"><span data-stu-id="019eb-182">Permissions sent by the [invite][] API may have additional information in the [invitation][SharingInvitation] facet.</span></span>
<span data-ttu-id="019eb-183">如果邀请发送给不匹配的已知的帐户的电子邮件地址， **grantedTo**属性可能不设置直到邀请会兑换，其中第一次用户单击的链接并登录时，发生此事件。</span><span class="sxs-lookup"><span data-stu-id="019eb-183">If an invitation was sent to an email address that doesn't match a known account, the **grantedTo** property may not be set until the invitation is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="019eb-184">在用户兑换共享邀请后，**grantedTo** 属性将包含兑换权限的帐户的相关信息：</span><span class="sxs-lookup"><span data-stu-id="019eb-184">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="019eb-185">方法</span><span class="sxs-lookup"><span data-stu-id="019eb-185">Methods</span></span>

| <span data-ttu-id="019eb-186">方法</span><span class="sxs-lookup"><span data-stu-id="019eb-186">Method</span></span>                                                   | <span data-ttu-id="019eb-187">REST 路径</span><span class="sxs-lookup"><span data-stu-id="019eb-187">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="019eb-188">列出权限</span><span class="sxs-lookup"><span data-stu-id="019eb-188">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="019eb-189">获取权限</span><span class="sxs-lookup"><span data-stu-id="019eb-189">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="019eb-190">[创建链接][createLink]</span><span class="sxs-lookup"><span data-stu-id="019eb-190">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="019eb-191">[邀请其他人][邀请]</span><span class="sxs-lookup"><span data-stu-id="019eb-191">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="019eb-192">更新</span><span class="sxs-lookup"><span data-stu-id="019eb-192">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="019eb-193">删除</span><span class="sxs-lookup"><span data-stu-id="019eb-193">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`



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
<!-- {
  "type": "#page.annotation",
  "description": "The permission object provides information about permissions and roles and sharing information.",
  "keywords": "sharing,permissions,read,write,acl",
  "section": "documentation",
  "tocPath": "Resources/Permission"
} -->
