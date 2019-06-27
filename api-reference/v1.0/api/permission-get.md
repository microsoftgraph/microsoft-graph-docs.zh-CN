---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取权限
localization_priority: Normal
ms.openlocfilehash: a2518745ea89e3d2192dae69ec4195d59ea31399
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275535"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="c52a8-102">获取文件或文件夹的共享权限</span><span class="sxs-lookup"><span data-stu-id="c52a8-102">Get sharing permission for a file or folder</span></span>

<span data-ttu-id="c52a8-103">返回特定 permission 资源的有效共享权限。</span><span class="sxs-lookup"><span data-stu-id="c52a8-103">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="c52a8-104">项的有效权限有两个来源：直接对项本身设置权限，或从项上级继承权限。</span><span class="sxs-lookup"><span data-stu-id="c52a8-104">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="c52a8-p101">调用方可以检查 `inheritedFrom` 属性来区分是否为继承权限。此属性是引用继承其权限的上级的 [ItemReference](../resources/itemreference.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="c52a8-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="c52a8-p102">对项设置的 SharePoint 权限级别在返回时包含“SP”前缀。 例如，SP.View Only、SP.Limited Access、SP.View Web Analytics Data。 请参阅 [SharePoint 角色完整列表](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1)。</span><span class="sxs-lookup"><span data-stu-id="c52a8-p102">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="c52a8-110">权限</span><span class="sxs-lookup"><span data-stu-id="c52a8-110">Permissions</span></span>

<span data-ttu-id="c52a8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c52a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c52a8-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c52a8-113">Permission type</span></span>      | <span data-ttu-id="c52a8-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c52a8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c52a8-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c52a8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c52a8-116">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c52a8-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c52a8-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c52a8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c52a8-118">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c52a8-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c52a8-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c52a8-119">Application</span></span> | <span data-ttu-id="c52a8-120">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c52a8-120">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c52a8-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c52a8-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c52a8-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c52a8-122">Optional query parameters</span></span>

<span data-ttu-id="c52a8-123">此方法支持 [$select 查询参数](/graph/query-parameters)塑造响应。</span><span class="sxs-lookup"><span data-stu-id="c52a8-123">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="c52a8-124">响应</span><span class="sxs-lookup"><span data-stu-id="c52a8-124">Response</span></span>

<span data-ttu-id="c52a8-125">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [权限](../resources/permission.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="c52a8-125">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c52a8-126">示例</span><span class="sxs-lookup"><span data-stu-id="c52a8-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="c52a8-127">请求</span><span class="sxs-lookup"><span data-stu-id="c52a8-127">Request</span></span>

<span data-ttu-id="c52a8-128">下面是请求访问某个文件夹权限的示例。</span><span class="sxs-lookup"><span data-stu-id="c52a8-128">Here is an example of the request to access a permission on a folder.</span></span>

<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="c52a8-129">响应</span><span class="sxs-lookup"><span data-stu-id="c52a8-129">Response</span></span>

<span data-ttu-id="c52a8-130">如果成功，此方法将返回特定 ID 的 [Permission](../resources/permission.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="c52a8-130">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c52a8-131">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c52a8-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c52a8-132">C#</span><span class="sxs-lookup"><span data-stu-id="c52a8-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-item-permission-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c52a8-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c52a8-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-item-permission-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c52a8-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="c52a8-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-item-permission-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="c52a8-135">注解</span><span class="sxs-lookup"><span data-stu-id="c52a8-135">Remarks</span></span>

<span data-ttu-id="c52a8-136">[权限](../resources/permission.md) 资源使用 _facet_ 提供有关由该资源表示的权限类型的信息。</span><span class="sxs-lookup"><span data-stu-id="c52a8-136">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="c52a8-p104">具有 [**链接**](../resources/sharinglink.md) facet 的权限表示在该项上创建的共享链接。共享链接包含一个唯一令牌，可以为具有上述链接的任何人提供对项目的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c52a8-p104">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="c52a8-139">具有 [**invitation**](../resources/sharinginvitation.md) facet 的权限表示通过邀请特定用户或组访问该文件添加的权限。</span><span class="sxs-lookup"><span data-stu-id="c52a8-139">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

### <a name="error-responses"></a><span data-ttu-id="c52a8-140">错误响应</span><span class="sxs-lookup"><span data-stu-id="c52a8-140">Error responses</span></span>

<span data-ttu-id="c52a8-141">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="c52a8-141">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
    "Error: /api-reference/v1.0/api/permission-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/permission-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/permission-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
