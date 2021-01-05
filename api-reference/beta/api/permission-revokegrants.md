---
title: permission： revokeGrants
description: 更新项目的共享权限
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e54d07f8d74a389f22f8f17b3d2eeabf74446eea
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753161"
---
# <a name="permission-revokegrants"></a><span data-ttu-id="3621f-103">permission： revokeGrants</span><span class="sxs-lookup"><span data-stu-id="3621f-103">permission: revokeGrants</span></span>
<span data-ttu-id="3621f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3621f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3621f-105">通过从链接中删除指定收件人，撤销对通过共享链接授予的[listItem][][或][][driveItem][]的访问权限。</span><span class="sxs-lookup"><span data-stu-id="3621f-105">Revoke access to a [listItem][] or [driveItem][] granted via a sharing link by removing the specified [recipient][] from the link.</span></span>

><span data-ttu-id="3621f-106">**注意：** 此功能仅适用于共享范围为用户的链接。</span><span class="sxs-lookup"><span data-stu-id="3621f-106">**Note:** This functionality is only available for sharing links scoped to users.</span></span>

[listItem]: ../resources/listitem.md
[driveItem]: ../resources/driveitem.md
[recipient]: ../resources/driverecipient.md

## <a name="permissions"></a><span data-ttu-id="3621f-110">权限</span><span class="sxs-lookup"><span data-stu-id="3621f-110">Permissions</span></span>
<span data-ttu-id="3621f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3621f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3621f-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="3621f-113">Permission type</span></span>|<span data-ttu-id="3621f-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3621f-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3621f-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3621f-115">Delegated (work or school account)</span></span>|<span data-ttu-id="3621f-116">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3621f-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>|
|<span data-ttu-id="3621f-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3621f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3621f-118">不支持</span><span class="sxs-lookup"><span data-stu-id="3621f-118">Not supported</span></span>|
|<span data-ttu-id="3621f-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="3621f-119">Application</span></span>|<span data-ttu-id="3621f-120">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3621f-120">Files.ReadWrite.All, Sites.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3621f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3621f-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /drives/{drive-id}/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/lists/{list-id}/items/{listItem-id}/permissions/{perm-id}/revokeGrants
POST /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
```

## <a name="request-headers"></a><span data-ttu-id="3621f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3621f-122">Request headers</span></span>
|<span data-ttu-id="3621f-123">名称</span><span class="sxs-lookup"><span data-stu-id="3621f-123">Name</span></span>|<span data-ttu-id="3621f-124">说明</span><span class="sxs-lookup"><span data-stu-id="3621f-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3621f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3621f-125">Authorization</span></span>|<span data-ttu-id="3621f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3621f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3621f-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3621f-128">Content-Type</span></span>|<span data-ttu-id="3621f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3621f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3621f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="3621f-131">Request body</span></span>
<span data-ttu-id="3621f-132">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3621f-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3621f-133">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="3621f-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3621f-134">参数</span><span class="sxs-lookup"><span data-stu-id="3621f-134">Parameter</span></span>|<span data-ttu-id="3621f-135">类型</span><span class="sxs-lookup"><span data-stu-id="3621f-135">Type</span></span>|<span data-ttu-id="3621f-136">说明</span><span class="sxs-lookup"><span data-stu-id="3621f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3621f-137">grantees</span><span class="sxs-lookup"><span data-stu-id="3621f-137">grantees</span></span>|<span data-ttu-id="3621f-138">[driveRecipient](../resources/driverecipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3621f-138">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="3621f-139">将撤消对共享链接的访问的收件人集合。</span><span class="sxs-lookup"><span data-stu-id="3621f-139">A collection of recipients who will be revoked access to the sharing link.</span></span>|

## <a name="response"></a><span data-ttu-id="3621f-140">响应</span><span class="sxs-lookup"><span data-stu-id="3621f-140">Response</span></span>

<span data-ttu-id="3621f-141">如果成功，此操作在响应正文中返回响应代码 `200 OK` 和权限。 [](../resources/permission.md)</span><span class="sxs-lookup"><span data-stu-id="3621f-141">If successful, this action returns a `200 OK` response code and a [permission](../resources/permission.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3621f-142">示例</span><span class="sxs-lookup"><span data-stu-id="3621f-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3621f-143">请求</span><span class="sxs-lookup"><span data-stu-id="3621f-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3621f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3621f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permission-revokegrants"
}
-->
``` http
POST /me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
Content-Type: application/json
Content-length: 95

{
  "grantees": [
    {
      "email": "ryan@contoso.com"
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="3621f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3621f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-revokegrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="3621f-146">C#</span><span class="sxs-lookup"><span data-stu-id="3621f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-revokegrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3621f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3621f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-revokegrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3621f-148">Java</span><span class="sxs-lookup"><span data-stu-id="3621f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permission-revokegrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3621f-149">响应</span><span class="sxs-lookup"><span data-stu-id="3621f-149">Response</span></span>

<span data-ttu-id="3621f-150">如果成功，此方法在响应正文中返回一个 [Permission](../resources/permission.md) 资源，该资源表示共享链接的更新状态。</span><span class="sxs-lookup"><span data-stu-id="3621f-150">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the sharing link.</span></span>

><span data-ttu-id="3621f-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3621f-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "users",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission"
} -->
