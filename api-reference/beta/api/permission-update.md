---
author: JeremyKelley
description: 通过修补 permission 资源更新共享权限的属性。
ms.date: 09/10/2017
title: 更改共享权限
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 3c5d0f45db2cf73c53adfd697840c2eb55c4c8c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455943"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="a97ca-103">更新共享权限</span><span class="sxs-lookup"><span data-stu-id="a97ca-103">Update sharing permission</span></span>

<span data-ttu-id="a97ca-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a97ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a97ca-105">通过修补 permission 资源更新共享权限的属性。</span><span class="sxs-lookup"><span data-stu-id="a97ca-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="a97ca-106">只有 **roles** 属性可以通过这种方式修改。</span><span class="sxs-lookup"><span data-stu-id="a97ca-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="a97ca-107">权限</span><span class="sxs-lookup"><span data-stu-id="a97ca-107">Permissions</span></span>

<span data-ttu-id="a97ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a97ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a97ca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a97ca-110">Permission type</span></span>      | <span data-ttu-id="a97ca-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a97ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a97ca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a97ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a97ca-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a97ca-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a97ca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a97ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a97ca-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a97ca-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a97ca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a97ca-116">Application</span></span> | <span data-ttu-id="a97ca-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a97ca-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a97ca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a97ca-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a97ca-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="a97ca-119">Optional request headers</span></span>

| <span data-ttu-id="a97ca-120">名称</span><span class="sxs-lookup"><span data-stu-id="a97ca-120">Name</span></span>          | <span data-ttu-id="a97ca-121">类型</span><span class="sxs-lookup"><span data-stu-id="a97ca-121">Type</span></span>   | <span data-ttu-id="a97ca-122">说明</span><span class="sxs-lookup"><span data-stu-id="a97ca-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a97ca-123">if-match</span><span class="sxs-lookup"><span data-stu-id="a97ca-123">if-match</span></span>      | <span data-ttu-id="a97ca-124">string</span><span class="sxs-lookup"><span data-stu-id="a97ca-124">string</span></span> | <span data-ttu-id="a97ca-125">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="a97ca-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a97ca-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a97ca-126">Request body</span></span>

<span data-ttu-id="a97ca-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a97ca-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="a97ca-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a97ca-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="a97ca-129">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="a97ca-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a97ca-130">属性</span><span class="sxs-lookup"><span data-stu-id="a97ca-130">Property</span></span>     | <span data-ttu-id="a97ca-131">类型</span><span class="sxs-lookup"><span data-stu-id="a97ca-131">Type</span></span>   | <span data-ttu-id="a97ca-132">说明</span><span class="sxs-lookup"><span data-stu-id="a97ca-132">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="a97ca-133">**角色**</span><span class="sxs-lookup"><span data-stu-id="a97ca-133">**roles**</span></span>    | <span data-ttu-id="a97ca-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="a97ca-134">String collection</span></span> | <span data-ttu-id="a97ca-135">权限类型的数组。</span><span class="sxs-lookup"><span data-stu-id="a97ca-135">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="a97ca-136">响应</span><span class="sxs-lookup"><span data-stu-id="a97ca-136">Response</span></span>

<span data-ttu-id="a97ca-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [permission](../resources/permission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a97ca-137">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a97ca-138">示例</span><span class="sxs-lookup"><span data-stu-id="a97ca-138">Example</span></span>

<span data-ttu-id="a97ca-139">下面是请求将共享权限上的角色更改为只读的示例。</span><span class="sxs-lookup"><span data-stu-id="a97ca-139">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="http"></a>[<span data-ttu-id="a97ca-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="a97ca-140">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="c"></a>[<span data-ttu-id="a97ca-141">C#</span><span class="sxs-lookup"><span data-stu-id="a97ca-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a97ca-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a97ca-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a97ca-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a97ca-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a97ca-144">响应</span><span class="sxs-lookup"><span data-stu-id="a97ca-144">Response</span></span>

<span data-ttu-id="a97ca-145">如果成功，此方法将在响应正文中返回 [Permission](../resources/permission.md) 资源，表示请求获取的更新后权限状态。</span><span class="sxs-lookup"><span data-stu-id="a97ca-145">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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
