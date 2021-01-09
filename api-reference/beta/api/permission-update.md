---
author: JeremyKelley
description: 通过修补 permission 资源更新共享权限的属性。
ms.date: 09/10/2017
title: 更改共享权限
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 56f9d600a36fb7b94757e6c783e2d397306e2de0
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790683"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="18e3b-103">更新共享权限</span><span class="sxs-lookup"><span data-stu-id="18e3b-103">Update sharing permission</span></span>

<span data-ttu-id="18e3b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18e3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18e3b-105">通过修补 permission 资源更新共享权限的属性。</span><span class="sxs-lookup"><span data-stu-id="18e3b-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="18e3b-106">只有 **roles** 属性可以通过这种方式修改。</span><span class="sxs-lookup"><span data-stu-id="18e3b-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="18e3b-107">权限</span><span class="sxs-lookup"><span data-stu-id="18e3b-107">Permissions</span></span>

<span data-ttu-id="18e3b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18e3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18e3b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="18e3b-110">Permission type</span></span>      | <span data-ttu-id="18e3b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18e3b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18e3b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18e3b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18e3b-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18e3b-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="18e3b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18e3b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18e3b-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18e3b-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="18e3b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="18e3b-116">Application</span></span> | <span data-ttu-id="18e3b-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18e3b-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18e3b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18e3b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="18e3b-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="18e3b-119">Optional request headers</span></span>

| <span data-ttu-id="18e3b-120">名称</span><span class="sxs-lookup"><span data-stu-id="18e3b-120">Name</span></span>          | <span data-ttu-id="18e3b-121">类型</span><span class="sxs-lookup"><span data-stu-id="18e3b-121">Type</span></span>   | <span data-ttu-id="18e3b-122">说明</span><span class="sxs-lookup"><span data-stu-id="18e3b-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="18e3b-123">if-match</span><span class="sxs-lookup"><span data-stu-id="18e3b-123">if-match</span></span>      | <span data-ttu-id="18e3b-124">string</span><span class="sxs-lookup"><span data-stu-id="18e3b-124">string</span></span> | <span data-ttu-id="18e3b-125">如果包含此请求标头，且提供的 eTag（或 cTag）与项中的当前标记不匹配，则返回 `412 Precondition Failed` 响应，并且不会删除该项。</span><span class="sxs-lookup"><span data-stu-id="18e3b-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18e3b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="18e3b-126">Request body</span></span>

<span data-ttu-id="18e3b-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="18e3b-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="18e3b-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="18e3b-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="18e3b-129">为了实现最佳性能，不得添加未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="18e3b-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="18e3b-130">可以修改这些权限类型的以下属性。</span><span class="sxs-lookup"><span data-stu-id="18e3b-130">The following properties on these permission types can be modified.</span></span>

| <span data-ttu-id="18e3b-131">权限类型</span><span class="sxs-lookup"><span data-stu-id="18e3b-131">Permission Type</span></span>        | <span data-ttu-id="18e3b-132">属性</span><span class="sxs-lookup"><span data-stu-id="18e3b-132">Property</span></span> | <span data-ttu-id="18e3b-133">类型</span><span class="sxs-lookup"><span data-stu-id="18e3b-133">Type</span></span>              | <span data-ttu-id="18e3b-134">说明</span><span class="sxs-lookup"><span data-stu-id="18e3b-134">Description</span></span>                   |
|:-----------------------|:---------|:------------------|:------------------------------|
| <span data-ttu-id="18e3b-135">用户</span><span class="sxs-lookup"><span data-stu-id="18e3b-135">User</span></span>                   | <span data-ttu-id="18e3b-136">角色</span><span class="sxs-lookup"><span data-stu-id="18e3b-136">roles</span></span>    | <span data-ttu-id="18e3b-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="18e3b-137">String collection</span></span> | <span data-ttu-id="18e3b-138">权限类型的数组。</span><span class="sxs-lookup"><span data-stu-id="18e3b-138">An array of permission types.</span></span> |
| <span data-ttu-id="18e3b-139">匿名共享链接</span><span class="sxs-lookup"><span data-stu-id="18e3b-139">Anonymous Sharing Link</span></span> | <span data-ttu-id="18e3b-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18e3b-140">expirationDateTime</span></span> | <span data-ttu-id="18e3b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18e3b-141">DateTimeOffset</span></span> | <span data-ttu-id="18e3b-142">权限过期时间的日期时间Offset 的 yyyy-MM-ddTHH：mm：ssZ 的格式。</span><span class="sxs-lookup"><span data-stu-id="18e3b-142">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset for the expiration time of the permission.</span></span> |

### <a name="remarks"></a><span data-ttu-id="18e3b-143">说明</span><span class="sxs-lookup"><span data-stu-id="18e3b-143">Remarks</span></span>
<span data-ttu-id="18e3b-144">不受支持的权限修改包括：</span><span class="sxs-lookup"><span data-stu-id="18e3b-144">Unsupported permission modifications include the following:</span></span>
- <span data-ttu-id="18e3b-145">组织共享链接</span><span class="sxs-lookup"><span data-stu-id="18e3b-145">Organizational sharing links</span></span>
- <span data-ttu-id="18e3b-146">人员共享链接</span><span class="sxs-lookup"><span data-stu-id="18e3b-146">People sharing links</span></span>

## <a name="response"></a><span data-ttu-id="18e3b-147">响应</span><span class="sxs-lookup"><span data-stu-id="18e3b-147">Response</span></span>

<span data-ttu-id="18e3b-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [permission](../resources/permission.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18e3b-148">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18e3b-149">示例</span><span class="sxs-lookup"><span data-stu-id="18e3b-149">Example</span></span>

<span data-ttu-id="18e3b-150">下面是请求将共享权限上的角色更改为只读的示例。</span><span class="sxs-lookup"><span data-stu-id="18e3b-150">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="http"></a>[<span data-ttu-id="18e3b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="18e3b-151">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="c"></a>[<span data-ttu-id="18e3b-152">C#</span><span class="sxs-lookup"><span data-stu-id="18e3b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18e3b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18e3b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18e3b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18e3b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18e3b-155">Java</span><span class="sxs-lookup"><span data-stu-id="18e3b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18e3b-156">响应</span><span class="sxs-lookup"><span data-stu-id="18e3b-156">Response</span></span>

<span data-ttu-id="18e3b-157">如果成功，此方法将在响应正文中返回 [Permission](../resources/permission.md) 资源，表示请求获取的更新后权限状态。</span><span class="sxs-lookup"><span data-stu-id="18e3b-157">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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


