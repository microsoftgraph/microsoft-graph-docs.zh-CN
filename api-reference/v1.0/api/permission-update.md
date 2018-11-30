---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 更改共享权限
ms.openlocfilehash: d6c710ca4d90bffba18cde316410480f1dde5821
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008912"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="942fe-102">更新共享权限</span><span class="sxs-lookup"><span data-stu-id="942fe-102">Update sharing permission</span></span>

<span data-ttu-id="942fe-103">通过修补 permission 资源更新共享权限的属性。</span><span class="sxs-lookup"><span data-stu-id="942fe-103">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="942fe-104">只有 **roles** 属性可以通过这种方式修改。</span><span class="sxs-lookup"><span data-stu-id="942fe-104">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="942fe-105">权限</span><span class="sxs-lookup"><span data-stu-id="942fe-105">Permissions</span></span>

<span data-ttu-id="942fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="942fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="942fe-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="942fe-108">Permission type</span></span>      | <span data-ttu-id="942fe-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="942fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="942fe-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="942fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="942fe-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942fe-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="942fe-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="942fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="942fe-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942fe-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="942fe-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="942fe-114">Application</span></span> | <span data-ttu-id="942fe-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942fe-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="942fe-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="942fe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="942fe-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="942fe-117">Optional request headers</span></span>

| <span data-ttu-id="942fe-118">名称</span><span class="sxs-lookup"><span data-stu-id="942fe-118">Name</span></span>          | <span data-ttu-id="942fe-119">类型</span><span class="sxs-lookup"><span data-stu-id="942fe-119">Type</span></span>   | <span data-ttu-id="942fe-120">说明</span><span class="sxs-lookup"><span data-stu-id="942fe-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="942fe-121">if-match</span><span class="sxs-lookup"><span data-stu-id="942fe-121">if-match</span></span>      | <span data-ttu-id="942fe-122">string</span><span class="sxs-lookup"><span data-stu-id="942fe-122">string</span></span> | <span data-ttu-id="942fe-123">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="942fe-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="942fe-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="942fe-124">Request body</span></span>

<span data-ttu-id="942fe-125">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="942fe-125">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="942fe-126">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="942fe-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="942fe-127">为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="942fe-127">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="942fe-128">属性</span><span class="sxs-lookup"><span data-stu-id="942fe-128">Property</span></span> | <span data-ttu-id="942fe-129">类型</span><span class="sxs-lookup"><span data-stu-id="942fe-129">Type</span></span>              | <span data-ttu-id="942fe-130">说明</span><span class="sxs-lookup"><span data-stu-id="942fe-130">Description</span></span>                   |
|:---------|:------------------|:------------------------------|
| <span data-ttu-id="942fe-131">roles</span><span class="sxs-lookup"><span data-stu-id="942fe-131">roles</span></span>    | <span data-ttu-id="942fe-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="942fe-132">String collection</span></span> | <span data-ttu-id="942fe-133">权限类型的数组。</span><span class="sxs-lookup"><span data-stu-id="942fe-133">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="942fe-134">响应</span><span class="sxs-lookup"><span data-stu-id="942fe-134">Response</span></span>

<span data-ttu-id="942fe-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [permission](../resources/permission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="942fe-135">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="942fe-136">示例</span><span class="sxs-lookup"><span data-stu-id="942fe-136">Example</span></span>

<span data-ttu-id="942fe-137">下面是请求将共享权限上的角色更改为只读的示例。</span><span class="sxs-lookup"><span data-stu-id="942fe-137">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- { "blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="942fe-138">响应</span><span class="sxs-lookup"><span data-stu-id="942fe-138">Response</span></span>

<span data-ttu-id="942fe-139">如果成功，此方法将在响应正文中返回 [Permission](../resources/permission.md) 资源，表示请求获取的更新后权限状态。</span><span class="sxs-lookup"><span data-stu-id="942fe-139">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="942fe-140">错误响应</span><span class="sxs-lookup"><span data-stu-id="942fe-140">Error responses</span></span>

<span data-ttu-id="942fe-141">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="942fe-141">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission"
} -->
