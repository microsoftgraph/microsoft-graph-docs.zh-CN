---
author: JeremyKelley
ms.author: JeremyKelley
title: 权限资源类型
description: 代表为 driveItem 授予的共享权限的权限资源
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c35134e39618121f9aa7b29c490a6d8427b4a373
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108198"
---
# <a name="permission-resource-type"></a><span data-ttu-id="514bf-103">权限资源类型</span><span class="sxs-lookup"><span data-stu-id="514bf-103">permission resource type</span></span>

<span data-ttu-id="514bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="514bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="514bf-105">**权限**资源提供了有关为[driveItem](driveitem.md)资源授予的共享权限的信息。</span><span class="sxs-lookup"><span data-stu-id="514bf-105">The **permission** resource provides information about a sharing permission granted for a [driveItem](driveitem.md) resource.</span></span>

<span data-ttu-id="514bf-106">共享权限具有许多不同的形式。</span><span class="sxs-lookup"><span data-stu-id="514bf-106">Sharing permissions have a number of different forms.</span></span>
<span data-ttu-id="514bf-107">**权限**资源通过资源上的 facet 表示这些不同的表单。</span><span class="sxs-lookup"><span data-stu-id="514bf-107">The **permission** resource represents these different forms through facets on the resource.</span></span>

><span data-ttu-id="514bf-108">**注意：** OneDrive for Business 和 SharePoint 文档库不返回**inheritedFrom**属性。</span><span class="sxs-lookup"><span data-stu-id="514bf-108">**Note:** OneDrive for Business and SharePoint document libraries do not return the **inheritedFrom** property.</span></span>

## <a name="json-representation"></a><span data-ttu-id="514bf-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="514bf-109">JSON representation</span></span>

<span data-ttu-id="514bf-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="514bf-110">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="514bf-111">属性</span><span class="sxs-lookup"><span data-stu-id="514bf-111">Properties</span></span>

| <span data-ttu-id="514bf-112">属性</span><span class="sxs-lookup"><span data-stu-id="514bf-112">Property</span></span>            | <span data-ttu-id="514bf-113">类型</span><span class="sxs-lookup"><span data-stu-id="514bf-113">Type</span></span>                        | <span data-ttu-id="514bf-114">说明</span><span class="sxs-lookup"><span data-stu-id="514bf-114">Description</span></span>
|:--------------------|:----------------------------|:-------------------------
| <span data-ttu-id="514bf-115">id</span><span class="sxs-lookup"><span data-stu-id="514bf-115">id</span></span>                  | <span data-ttu-id="514bf-116">字符串</span><span class="sxs-lookup"><span data-stu-id="514bf-116">String</span></span>                      | <span data-ttu-id="514bf-p102">在项目的所有权限中，某个权限的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="514bf-p102">The unique identifier of the permission among all permissions on the item. Read-only.</span></span>
| <span data-ttu-id="514bf-119">grantedTo</span><span class="sxs-lookup"><span data-stu-id="514bf-119">grantedTo</span></span>           | <span data-ttu-id="514bf-120">[IdentitySet][]</span><span class="sxs-lookup"><span data-stu-id="514bf-120">[IdentitySet][]</span></span>             | <span data-ttu-id="514bf-p103">对于用户类型权限，此权限的用户和应用程序的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="514bf-p103">For user type permissions, the details of the users & applications for this permission. Read-only.</span></span>
| <span data-ttu-id="514bf-123">grantedToIdentities</span><span class="sxs-lookup"><span data-stu-id="514bf-123">grantedToIdentities</span></span> | <span data-ttu-id="514bf-124">Collection([IdentitySet][])</span><span class="sxs-lookup"><span data-stu-id="514bf-124">Collection([IdentitySet][])</span></span> | <span data-ttu-id="514bf-125">对于链接类型权限，被授予权限的用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="514bf-125">For link type permissions, the details of the users to whom permission was granted.</span></span> <span data-ttu-id="514bf-126">只读。</span><span class="sxs-lookup"><span data-stu-id="514bf-126">Read-only.</span></span>
| <span data-ttu-id="514bf-127">invitation</span><span class="sxs-lookup"><span data-stu-id="514bf-127">invitation</span></span>          | <span data-ttu-id="514bf-128">[SharingInvitation][]</span><span class="sxs-lookup"><span data-stu-id="514bf-128">[SharingInvitation][]</span></span>       | <span data-ttu-id="514bf-p105">此权限的全部关联共享邀请的详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="514bf-p105">Details of any associated sharing invitation for this permission. Read-only.</span></span>
| <span data-ttu-id="514bf-131">inheritedFrom</span><span class="sxs-lookup"><span data-stu-id="514bf-131">inheritedFrom</span></span>       | <span data-ttu-id="514bf-132">[ItemReference][]</span><span class="sxs-lookup"><span data-stu-id="514bf-132">[ItemReference][]</span></span>           | <span data-ttu-id="514bf-p106">如果当前权限继承自上级，则提供对当前权限的上级的引用。只读。</span><span class="sxs-lookup"><span data-stu-id="514bf-p106">Provides a reference to the ancestor of the current permission, if it is inherited from an ancestor. Read-only.</span></span>
| <span data-ttu-id="514bf-135">link</span><span class="sxs-lookup"><span data-stu-id="514bf-135">link</span></span>                | <span data-ttu-id="514bf-136">[SharingLink][]</span><span class="sxs-lookup"><span data-stu-id="514bf-136">[SharingLink][]</span></span>             | <span data-ttu-id="514bf-p107">如果当前权限是链接类型权限，则提供当前权限的链接详细信息。只读。</span><span class="sxs-lookup"><span data-stu-id="514bf-p107">Provides the link details of the current permission, if it is a link type permissions. Read-only.</span></span>
| <span data-ttu-id="514bf-139">角色</span><span class="sxs-lookup"><span data-stu-id="514bf-139">roles</span></span>               | <span data-ttu-id="514bf-140">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="514bf-140">Collection(String)</span></span>          | <span data-ttu-id="514bf-p108">权限类型，例如 `read`。有关角色的完整列表，请参阅如下内容。只读。</span><span class="sxs-lookup"><span data-stu-id="514bf-p108">The type of permission, e.g. `read`. See below for the full list of roles. Read-only.</span></span>
| <span data-ttu-id="514bf-144">shareId</span><span class="sxs-lookup"><span data-stu-id="514bf-144">shareId</span></span>             | <span data-ttu-id="514bf-145">String</span><span class="sxs-lookup"><span data-stu-id="514bf-145">String</span></span>                      | <span data-ttu-id="514bf-146">可用于通过 **[shares API][]** 访问此共享项的唯一令牌。</span><span class="sxs-lookup"><span data-stu-id="514bf-146">A unique token that can be used to access this shared item via the **[shares API][]**.</span></span> <span data-ttu-id="514bf-147">只读。</span><span class="sxs-lookup"><span data-stu-id="514bf-147">Read-only.</span></span>
| <span data-ttu-id="514bf-148">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="514bf-148">expirationDateTime</span></span>  | <span data-ttu-id="514bf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="514bf-149">DateTimeOffset</span></span>              | <span data-ttu-id="514bf-150">Yyyy-mm-ddthh： MM： ssZ of DateTimeOffset 的格式指示权限的过期时间。</span><span class="sxs-lookup"><span data-stu-id="514bf-150">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset indicates the expiration time of the permission.</span></span> <span data-ttu-id="514bf-151">MinValue 指示此权限没有设置过期时间。</span><span class="sxs-lookup"><span data-stu-id="514bf-151">DateTime.MinValue indicates there is no expiration set for this permission.</span></span> <span data-ttu-id="514bf-152">可选。</span><span class="sxs-lookup"><span data-stu-id="514bf-152">Optional.</span></span>
| <span data-ttu-id="514bf-153">hasPassword</span><span class="sxs-lookup"><span data-stu-id="514bf-153">hasPassword</span></span>         | <span data-ttu-id="514bf-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="514bf-154">Boolean</span></span>                     | <span data-ttu-id="514bf-155">这指示是否为此权限设置了密码，它仅显示为 "响应"。</span><span class="sxs-lookup"><span data-stu-id="514bf-155">This indicates whether password is set for this permission, it's only showing in response.</span></span> <span data-ttu-id="514bf-156">可选和只读，仅适用于 OneDrive 个人版。</span><span class="sxs-lookup"><span data-stu-id="514bf-156">Optional and Read-only and for OneDrive Personal only.</span></span>

### <a name="roles-enumeration-values"></a><span data-ttu-id="514bf-157">角色枚举值</span><span class="sxs-lookup"><span data-stu-id="514bf-157">Roles enumeration values</span></span>

| <span data-ttu-id="514bf-158">值</span><span class="sxs-lookup"><span data-stu-id="514bf-158">Value</span></span>        | <span data-ttu-id="514bf-159">详细信息</span><span class="sxs-lookup"><span data-stu-id="514bf-159">Details</span></span>                                                                        |
|:------------|:-------------------------------------------------------------------------------|
| `read`      | <span data-ttu-id="514bf-160">提供读取项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="514bf-160">Provides the ability to read the metadata and contents of the item.</span></span>            |
| `write`     | <span data-ttu-id="514bf-161">提供读取并修改项的元数据和内容的功能。</span><span class="sxs-lookup"><span data-stu-id="514bf-161">Provides the ability to read and modify the metadata and contents of the item.</span></span> |
| `sp.owner`  | <span data-ttu-id="514bf-162">对于 SharePoint 和 OneDrive for Business，这表示所有者角色。</span><span class="sxs-lookup"><span data-stu-id="514bf-162">For SharePoint and OneDrive for Business this represents the owner role.</span></span>       |
| `sp.member` | <span data-ttu-id="514bf-163">对于 SharePoint 和 OneDrive for Business，这表示成员角色。</span><span class="sxs-lookup"><span data-stu-id="514bf-163">For SharePoint and OneDrive for Business this represents the member role.</span></span>      |

<span data-ttu-id="514bf-164">权限资源使用 _facet_ 提供有关由该资源表示的权限类型的信息。</span><span class="sxs-lookup"><span data-stu-id="514bf-164">The permission resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="514bf-165">共享链接包含访问该项所需的唯一令牌。</span><span class="sxs-lookup"><span data-stu-id="514bf-165">Sharing links contain a unique token required to access the item.</span></span>

<span data-ttu-id="514bf-166">具有[**邀请**][SharingInvitation] facet 的权限表示通过邀请特定用户或组访问文件而添加的权限。</span><span class="sxs-lookup"><span data-stu-id="514bf-166">Permissions with an [**invitation**][SharingInvitation] facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

## <a name="sharing-links"></a><span data-ttu-id="514bf-167">共享链接</span><span class="sxs-lookup"><span data-stu-id="514bf-167">Sharing links</span></span>

<span data-ttu-id="514bf-168">具有[**链接**][SharingLink] facet 的权限表示在该项上创建的共享链接。</span><span class="sxs-lookup"><span data-stu-id="514bf-168">Permissions with a [**link**][SharingLink] facet represent sharing links created on the item.</span></span>
<span data-ttu-id="514bf-169">这些是最常见的权限类型。</span><span class="sxs-lookup"><span data-stu-id="514bf-169">These are the most common kinds of permissions.</span></span>
<span data-ttu-id="514bf-170">共享链接提供可用于访问文件或文件夹的唯一 URL。</span><span class="sxs-lookup"><span data-stu-id="514bf-170">Sharing links provide a unique URL that can be used to access a file or folder.</span></span>
<span data-ttu-id="514bf-171">可将其设置为通过多种方式授予访问权限。</span><span class="sxs-lookup"><span data-stu-id="514bf-171">They can be set up to grant access in a variety of ways.</span></span>
<span data-ttu-id="514bf-172">例如，可使用 [createLink][] API 创建适用于已登录到组织的任何用户的链接，或创建可用于任何人且无需登录的链接。</span><span class="sxs-lookup"><span data-stu-id="514bf-172">For example, you can use the [createLink][] API to create a link that works for anyone signed into your organization, or you can create a link that works for anyone, without needing to sign in.</span></span>
<span data-ttu-id="514bf-173">你可以使用 [invite][] API 创建仅适用于特定人员的链接（无论他们是否在你的公司中）。</span><span class="sxs-lookup"><span data-stu-id="514bf-173">You can use the [invite][] API to create a link that only works for specific people, whether they're in your company or not.</span></span>

<span data-ttu-id="514bf-174">下面是一些共享链接示例。</span><span class="sxs-lookup"><span data-stu-id="514bf-174">Here are some examples of sharing links.</span></span>

### <a name="view-link"></a><span data-ttu-id="514bf-175">查看链接</span><span class="sxs-lookup"><span data-stu-id="514bf-175">View link</span></span>

<span data-ttu-id="514bf-176">此查看链接向具有相应链接的任何人提供只读访问权限。</span><span class="sxs-lookup"><span data-stu-id="514bf-176">This view link provides read-only access to anyone with the link.</span></span>

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

### <a name="edit-link"></a><span data-ttu-id="514bf-177">编辑链接</span><span class="sxs-lookup"><span data-stu-id="514bf-177">Edit link</span></span>

<span data-ttu-id="514bf-178">此编辑链接向组织中具有相应链接的任何人提供读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="514bf-178">This edit link provides read and write access to anyone in the organization with the link.</span></span>

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

### <a name="existing-access-link"></a><span data-ttu-id="514bf-179">现有访问链接</span><span class="sxs-lookup"><span data-stu-id="514bf-179">Existing access link</span></span>

<span data-ttu-id="514bf-180">此链接不向用户授予任何其他权限。</span><span class="sxs-lookup"><span data-stu-id="514bf-180">This link does not grant any additional privileges to the user.</span></span>

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

### <a name="specific-people-link"></a><span data-ttu-id="514bf-181">特定人员链接</span><span class="sxs-lookup"><span data-stu-id="514bf-181">Specific people link</span></span>

<span data-ttu-id="514bf-182">此链接向 `grantedToIdentities` 集合中的特定人员提供读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="514bf-182">This link provides read and write access to the specific people in the `grantedToIdentities` collection.</span></span>

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

## <a name="sharing-invitations"></a><span data-ttu-id="514bf-183">共享邀请</span><span class="sxs-lookup"><span data-stu-id="514bf-183">Sharing invitations</span></span>

<span data-ttu-id="514bf-184">由[邀请][]或[授予][]API 发送的权限可以在[邀请][SharingInvitation] facet 中为不匹配已知帐户的电子邮件地址提供其他信息。</span><span class="sxs-lookup"><span data-stu-id="514bf-184">Permissions sent by the [invite][] or [grant][] API can have additional information in the [invitation][SharingInvitation] facet for email addresses that don't match a known account.</span></span> <span data-ttu-id="514bf-185">在这种情况下， **grantedTo**属性可能不会设置，直到该邀请链接被兑换（当用户首次单击该链接并登录）时才会发生此事件。</span><span class="sxs-lookup"><span data-stu-id="514bf-185">In such cases, the **grantedTo** property might not be set until the invitation link is redeemed, which occurs the first time the user clicks the link and signs in.</span></span>

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

<span data-ttu-id="514bf-186">在用户兑换共享邀请后，**grantedTo** 属性将包含兑换权限的帐户的相关信息：</span><span class="sxs-lookup"><span data-stu-id="514bf-186">After the sharing invitation has been redeemed by a user, the **grantedTo** property will contain the information about the account that redeemed the permissions:</span></span>

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

## <a name="methods"></a><span data-ttu-id="514bf-187">方法</span><span class="sxs-lookup"><span data-stu-id="514bf-187">Methods</span></span>

| <span data-ttu-id="514bf-188">方法</span><span class="sxs-lookup"><span data-stu-id="514bf-188">Method</span></span>                                                   | <span data-ttu-id="514bf-189">REST 路径</span><span class="sxs-lookup"><span data-stu-id="514bf-189">REST Path</span></span>
|:---------------------------------------------------------|:-----------------------
| [<span data-ttu-id="514bf-190">列出权限</span><span class="sxs-lookup"><span data-stu-id="514bf-190">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="514bf-191">获取权限</span><span class="sxs-lookup"><span data-stu-id="514bf-191">Get permission</span></span>](../api/permission-get.md)               | `GET /drive/items/{item-id}/permissions/{id}`
| <span data-ttu-id="514bf-192">[创建链接][createLink]</span><span class="sxs-lookup"><span data-stu-id="514bf-192">[Create link][createLink]</span></span>                                | `POST /drive/items/{item-id}/createLink`
| <span data-ttu-id="514bf-193">[邀请人员][invite]</span><span class="sxs-lookup"><span data-stu-id="514bf-193">[Invite people][invite]</span></span>                                  | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="514bf-194">更新</span><span class="sxs-lookup"><span data-stu-id="514bf-194">Update</span></span>](../api/permission-update.md)                    | `PATCH /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="514bf-195">删除</span><span class="sxs-lookup"><span data-stu-id="514bf-195">Delete</span></span>](../api/permission-delete.md)                    | `DELETE /drive/items/{item-id}/permissions/{id}`
| [<span data-ttu-id="514bf-196">将用户添加到共享链接</span><span class="sxs-lookup"><span data-stu-id="514bf-196">Add users to sharing link</span></span>](../api/permission-grant.md)  | `POST /shares/{encoded-sharing-url}/permission/grant`


[createLink]: ../api/driveitem-createlink.md
[授]: ../api/permission-grant.md
[grant]: ../api/permission-grant.md
[IdentitySet]: identityset.md
[invite]: ../api/driveitem-invite.md
[ItemReference]: itemreference.md
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
  "suppressions": []
}
-->
