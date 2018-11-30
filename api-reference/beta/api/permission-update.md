---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 更改共享权限
ms.openlocfilehash: 96662cac4a58dcff9ed7faa40f61c8a09bfc88b3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041252"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="28c9d-102">更新共享权限</span><span class="sxs-lookup"><span data-stu-id="28c9d-102">Update sharing permission</span></span>

> <span data-ttu-id="28c9d-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="28c9d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28c9d-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="28c9d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28c9d-105">通过修补 permission 资源更新共享权限的属性。</span><span class="sxs-lookup"><span data-stu-id="28c9d-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="28c9d-106">只有 **roles** 属性可以通过这种方式修改。</span><span class="sxs-lookup"><span data-stu-id="28c9d-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="28c9d-107">权限</span><span class="sxs-lookup"><span data-stu-id="28c9d-107">Permissions</span></span>

<span data-ttu-id="28c9d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28c9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28c9d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="28c9d-110">Permission type</span></span>      | <span data-ttu-id="28c9d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28c9d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28c9d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28c9d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="28c9d-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c9d-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="28c9d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28c9d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28c9d-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c9d-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="28c9d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="28c9d-116">Application</span></span> | <span data-ttu-id="28c9d-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c9d-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28c9d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28c9d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="28c9d-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="28c9d-119">Optional request headers</span></span>

| <span data-ttu-id="28c9d-120">名称</span><span class="sxs-lookup"><span data-stu-id="28c9d-120">Name</span></span>          | <span data-ttu-id="28c9d-121">类型</span><span class="sxs-lookup"><span data-stu-id="28c9d-121">Type</span></span>   | <span data-ttu-id="28c9d-122">说明</span><span class="sxs-lookup"><span data-stu-id="28c9d-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="28c9d-123">if-match</span><span class="sxs-lookup"><span data-stu-id="28c9d-123">if-match</span></span>      | <span data-ttu-id="28c9d-124">string</span><span class="sxs-lookup"><span data-stu-id="28c9d-124">string</span></span> | <span data-ttu-id="28c9d-125">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="28c9d-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28c9d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28c9d-126">Request body</span></span>

<span data-ttu-id="28c9d-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="28c9d-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="28c9d-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="28c9d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="28c9d-129">为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="28c9d-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="28c9d-130">属性</span><span class="sxs-lookup"><span data-stu-id="28c9d-130">Property</span></span>     | <span data-ttu-id="28c9d-131">类型</span><span class="sxs-lookup"><span data-stu-id="28c9d-131">Type</span></span>   | <span data-ttu-id="28c9d-132">说明</span><span class="sxs-lookup"><span data-stu-id="28c9d-132">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="28c9d-133">**角色**</span><span class="sxs-lookup"><span data-stu-id="28c9d-133">**roles**</span></span>    | <span data-ttu-id="28c9d-134">String</span><span class="sxs-lookup"><span data-stu-id="28c9d-134">String</span></span> | <span data-ttu-id="28c9d-135">权限类型的数组。</span><span class="sxs-lookup"><span data-stu-id="28c9d-135">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="28c9d-136">响应</span><span class="sxs-lookup"><span data-stu-id="28c9d-136">Response</span></span>

<span data-ttu-id="28c9d-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [permission](../resources/permission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28c9d-137">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28c9d-138">示例</span><span class="sxs-lookup"><span data-stu-id="28c9d-138">Example</span></span>

<span data-ttu-id="28c9d-139">下面是请求将共享权限上的角色更改为只读的示例。</span><span class="sxs-lookup"><span data-stu-id="28c9d-139">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="28c9d-140">响应</span><span class="sxs-lookup"><span data-stu-id="28c9d-140">Response</span></span>

<span data-ttu-id="28c9d-141">如果成功，此方法将在响应正文中返回 [Permission](../resources/permission.md) 资源，表示请求获取的更新后权限状态。</span><span class="sxs-lookup"><span data-stu-id="28c9d-141">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
