---
author: JeremyKelley
description: 返回特定 permission 资源的有效共享权限。
ms.date: 09/10/2017
title: 获取权限
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 522c4b4bcaefb74933c41afc37506917e54fd89e
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635500"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="b52ee-103">获取文件或文件夹的共享权限</span><span class="sxs-lookup"><span data-stu-id="b52ee-103">Get sharing permission for a file or folder</span></span>

<span data-ttu-id="b52ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b52ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b52ee-105">返回特定 permission 资源的有效共享权限。</span><span class="sxs-lookup"><span data-stu-id="b52ee-105">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="b52ee-106">项的有效权限有两个来源：直接对项本身设置权限，或从项上级继承权限。</span><span class="sxs-lookup"><span data-stu-id="b52ee-106">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="b52ee-p101">调用方可以检查 `inheritedFrom` 属性来区分是否为继承权限。此属性是引用继承其权限的上级的 [ItemReference](../resources/itemreference.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="b52ee-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="b52ee-p102">对项设置的 SharePoint 权限级别在返回时包含“SP”前缀。 例如，SP.View Only、SP.Limited Access、SP.View Web Analytics Data。 请参阅 [SharePoint 角色完整列表](/SharePoint/sites/user-permissions-and-permission-levels#section1)。</span><span class="sxs-lookup"><span data-stu-id="b52ee-p102">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](/SharePoint/sites/user-permissions-and-permission-levels#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="b52ee-112">权限</span><span class="sxs-lookup"><span data-stu-id="b52ee-112">Permissions</span></span>

<span data-ttu-id="b52ee-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b52ee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b52ee-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="b52ee-115">Permission type</span></span>      | <span data-ttu-id="b52ee-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b52ee-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b52ee-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b52ee-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b52ee-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b52ee-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b52ee-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b52ee-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b52ee-120">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b52ee-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b52ee-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="b52ee-121">Application</span></span> | <span data-ttu-id="b52ee-122">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b52ee-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b52ee-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b52ee-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b52ee-124">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="b52ee-124">Optional query parameters</span></span>

<span data-ttu-id="b52ee-125">此方法支持 [$select 查询参数](/graph/query-parameters)塑造响应。</span><span class="sxs-lookup"><span data-stu-id="b52ee-125">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="b52ee-126">响应</span><span class="sxs-lookup"><span data-stu-id="b52ee-126">Response</span></span>

<span data-ttu-id="b52ee-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [权限](../resources/permission.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="b52ee-127">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b52ee-128">示例</span><span class="sxs-lookup"><span data-stu-id="b52ee-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="b52ee-129">请求</span><span class="sxs-lookup"><span data-stu-id="b52ee-129">Request</span></span>

<span data-ttu-id="b52ee-130">下面是请求访问某个文件夹权限的示例。</span><span class="sxs-lookup"><span data-stu-id="b52ee-130">Here is an example of the request to access a permission on a folder.</span></span>


# <a name="http"></a>[<span data-ttu-id="b52ee-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b52ee-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```
# <a name="c"></a>[<span data-ttu-id="b52ee-132">C#</span><span class="sxs-lookup"><span data-stu-id="b52ee-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b52ee-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b52ee-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b52ee-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b52ee-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b52ee-135">响应</span><span class="sxs-lookup"><span data-stu-id="b52ee-135">Response</span></span>

<span data-ttu-id="b52ee-136">如果成功，此方法将返回特定 ID 的 [Permission](../resources/permission.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="b52ee-136">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

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

## <a name="remarks"></a><span data-ttu-id="b52ee-137">注解</span><span class="sxs-lookup"><span data-stu-id="b52ee-137">Remarks</span></span>

<span data-ttu-id="b52ee-138">[权限](../resources/permission.md) 资源使用 _facet_ 提供有关由该资源表示的权限类型的信息。</span><span class="sxs-lookup"><span data-stu-id="b52ee-138">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="b52ee-p104">具有 [**链接**](../resources/sharinglink.md) facet 的权限表示在该项上创建的共享链接。共享链接包含一个唯一令牌，可以为具有上述链接的任何人提供对项目的访问权限。</span><span class="sxs-lookup"><span data-stu-id="b52ee-p104">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="b52ee-141">具有 [**邀请**](../resources/sharinginvitation.md) facet 的权限表示通过邀请特定用户或组访问该文件添加的权限。</span><span class="sxs-lookup"><span data-stu-id="b52ee-141">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission",
  "suppressions": [
  ]
}
-->
