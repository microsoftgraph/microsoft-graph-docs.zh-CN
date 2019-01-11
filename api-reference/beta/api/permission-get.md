---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 获取权限
localization_priority: Normal
ms.openlocfilehash: efc92c94350f391c980e72cf57fb8ad12108a832
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808349"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="8b2a2-102">获取文件或文件夹的共享权限</span><span class="sxs-lookup"><span data-stu-id="8b2a2-102">Get sharing permission for a file or folder</span></span>

> <span data-ttu-id="8b2a2-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b2a2-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b2a2-105">返回特定 permission 资源的有效共享权限。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-105">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="8b2a2-106">项的有效权限有两个来源：直接对项本身设置权限，或从项上级继承权限。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-106">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="8b2a2-p102">调用方可以检查 `inheritedFrom` 属性来区分是否为继承权限。此属性是引用继承其权限的上级的 [ItemReference](../resources/itemreference.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-p102">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="8b2a2-109">对项设置的 SharePoint 权限级别在返回时包含“SP”前缀。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-109">SharePoint permission levels set on an item are returned with an 'SP' prefix.</span></span> <span data-ttu-id="8b2a2-110">例如，SP.View Only、SP.Limited Access、SP.View Web Analytics Data。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-110">For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data.</span></span> <span data-ttu-id="8b2a2-111">请参阅 [SharePoint 角色完整列表](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-111">See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="8b2a2-112">权限</span><span class="sxs-lookup"><span data-stu-id="8b2a2-112">Permissions</span></span>

<span data-ttu-id="8b2a2-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b2a2-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b2a2-115">Permission type</span></span>      | <span data-ttu-id="8b2a2-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b2a2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b2a2-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b2a2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="8b2a2-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b2a2-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b2a2-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b2a2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b2a2-120">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b2a2-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b2a2-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b2a2-121">Application</span></span> | <span data-ttu-id="8b2a2-122">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b2a2-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b2a2-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b2a2-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b2a2-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8b2a2-124">Optional query parameters</span></span>

<span data-ttu-id="8b2a2-125">此方法支持 [$select 查询参数](/graph/query-parameters)塑造响应。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-125">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="8b2a2-126">响应</span><span class="sxs-lookup"><span data-stu-id="8b2a2-126">Response</span></span>

<span data-ttu-id="8b2a2-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [权限](../resources/permission.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-127">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b2a2-128">示例</span><span class="sxs-lookup"><span data-stu-id="8b2a2-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b2a2-129">请求</span><span class="sxs-lookup"><span data-stu-id="8b2a2-129">Request</span></span>

<span data-ttu-id="8b2a2-130">下面是请求访问某个文件夹权限的示例。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-130">Here is an example of the request to access a permission on a folder.</span></span>

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```
### <a name="response"></a><span data-ttu-id="8b2a2-131">响应</span><span class="sxs-lookup"><span data-stu-id="8b2a2-131">Response</span></span>

<span data-ttu-id="8b2a2-132">如果成功，此方法将返回特定 ID 的 [Permission](../resources/permission.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-132">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="8b2a2-133">备注</span><span class="sxs-lookup"><span data-stu-id="8b2a2-133">Remarks</span></span>

<span data-ttu-id="8b2a2-134">[权限](../resources/permission.md) 资源使用 _facet_ 提供有关由该资源表示的权限类型的信息。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-134">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="8b2a2-p105">具有 [**链接**](../resources/sharinglink.md) facet 的权限表示在该项上创建的共享链接。共享链接包含一个唯一令牌，可以为具有上述链接的任何人提供对项目的访问权限。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-p105">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="8b2a2-137">具有 [**邀请**](../resources/sharinginvitation.md) facet 的权限表示通过邀请特定用户或组访问该文件添加的权限。</span><span class="sxs-lookup"><span data-stu-id="8b2a2-137">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission"
}-->
