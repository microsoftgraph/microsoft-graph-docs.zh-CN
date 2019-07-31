---
author: JeremyKelley
description: 通过修补 permission 资源更新共享权限的属性。
ms.date: 09/10/2017
title: 更改共享权限
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: ef46b64db30c6d8ceaf65a2f4a7f4c935834b9b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983493"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="d2ecc-103">更新共享权限</span><span class="sxs-lookup"><span data-stu-id="d2ecc-103">Update sharing permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2ecc-104">通过修补 permission 资源更新共享权限的属性。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-104">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="d2ecc-105">只有 **roles** 属性可以通过这种方式修改。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-105">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2ecc-106">权限</span><span class="sxs-lookup"><span data-stu-id="d2ecc-106">Permissions</span></span>

<span data-ttu-id="d2ecc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2ecc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2ecc-109">Permission type</span></span>      | <span data-ttu-id="d2ecc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2ecc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2ecc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2ecc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2ecc-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2ecc-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2ecc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2ecc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2ecc-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2ecc-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2ecc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2ecc-115">Application</span></span> | <span data-ttu-id="d2ecc-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2ecc-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2ecc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2ecc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="d2ecc-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="d2ecc-118">Optional request headers</span></span>

| <span data-ttu-id="d2ecc-119">名称</span><span class="sxs-lookup"><span data-stu-id="d2ecc-119">Name</span></span>          | <span data-ttu-id="d2ecc-120">类型</span><span class="sxs-lookup"><span data-stu-id="d2ecc-120">Type</span></span>   | <span data-ttu-id="d2ecc-121">说明</span><span class="sxs-lookup"><span data-stu-id="d2ecc-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d2ecc-122">if-match</span><span class="sxs-lookup"><span data-stu-id="d2ecc-122">if-match</span></span>      | <span data-ttu-id="d2ecc-123">string</span><span class="sxs-lookup"><span data-stu-id="d2ecc-123">string</span></span> | <span data-ttu-id="d2ecc-124">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2ecc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2ecc-125">Request body</span></span>

<span data-ttu-id="d2ecc-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-126">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="d2ecc-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="d2ecc-128">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d2ecc-129">属性</span><span class="sxs-lookup"><span data-stu-id="d2ecc-129">Property</span></span>     | <span data-ttu-id="d2ecc-130">类型</span><span class="sxs-lookup"><span data-stu-id="d2ecc-130">Type</span></span>   | <span data-ttu-id="d2ecc-131">说明</span><span class="sxs-lookup"><span data-stu-id="d2ecc-131">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="d2ecc-132">**角色**</span><span class="sxs-lookup"><span data-stu-id="d2ecc-132">**roles**</span></span>    | <span data-ttu-id="d2ecc-133">String collection</span><span class="sxs-lookup"><span data-stu-id="d2ecc-133">String collection</span></span> | <span data-ttu-id="d2ecc-134">权限类型的数组。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-134">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="d2ecc-135">响应</span><span class="sxs-lookup"><span data-stu-id="d2ecc-135">Response</span></span>

<span data-ttu-id="d2ecc-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [permission](../resources/permission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-136">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2ecc-137">示例</span><span class="sxs-lookup"><span data-stu-id="d2ecc-137">Example</span></span>

<span data-ttu-id="d2ecc-138">下面是请求将共享权限上的角色更改为只读的示例。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-138">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d2ecc-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d2ecc-139">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2ecc-140">C#</span><span class="sxs-lookup"><span data-stu-id="d2ecc-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2ecc-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2ecc-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2ecc-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="d2ecc-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2ecc-143">Java</span><span class="sxs-lookup"><span data-stu-id="d2ecc-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2ecc-144">响应</span><span class="sxs-lookup"><span data-stu-id="d2ecc-144">Response</span></span>

<span data-ttu-id="d2ecc-145">如果成功，此方法将在响应正文中返回 [Permission](../resources/permission.md) 资源，表示请求获取的更新后权限状态。</span><span class="sxs-lookup"><span data-stu-id="d2ecc-145">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true } -->

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
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission",
  "suppressions": [
  ]
}
-->
