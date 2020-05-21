---
title: 向用户授予 appRoleAssignment
description: 向用户授予应用程序角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c6a34fa1116b5679c70997913b93b74d41b9e459
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332478"
---
# <a name="grant-an-approleassignment-to-a-user"></a><span data-ttu-id="50833-103">向用户授予 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="50833-103">Grant an appRoleAssignment to a user</span></span>

<span data-ttu-id="50833-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50833-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50833-105">使用此 API 将应用程序角色分配给用户。</span><span class="sxs-lookup"><span data-stu-id="50833-105">Use this API to assign an app role to a user.</span></span> <span data-ttu-id="50833-106">若要向用户授予应用程序角色分配，需要三个标识符：</span><span class="sxs-lookup"><span data-stu-id="50833-106">To grant an app role assignment to a user, you need three identifiers:</span></span>

- <span data-ttu-id="50833-107">`principalId`：要 `id` 向其分配应用程序角色的用户。</span><span class="sxs-lookup"><span data-stu-id="50833-107">`principalId`: The `id` of the user to whom you are assigning the app role.</span></span>
- <span data-ttu-id="50833-108">`resourceId`： `id` `servicePrincipal` 定义了应用程序角色的资源的。</span><span class="sxs-lookup"><span data-stu-id="50833-108">`resourceId`: The `id` of the resource `servicePrincipal` that has defined the app role.</span></span>
- <span data-ttu-id="50833-109">`appRoleId`： `id` `appRole` 要分配给用户的（在资源服务主体上定义）的。</span><span class="sxs-lookup"><span data-stu-id="50833-109">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="50833-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="50833-110">Permissions</span></span>

<span data-ttu-id="50833-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50833-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50833-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="50833-113">Permission type</span></span>      | <span data-ttu-id="50833-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50833-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50833-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50833-115">Delegated (work or school account)</span></span> | <span data-ttu-id="50833-116">AppRoleAssignment、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="50833-116">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50833-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50833-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50833-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="50833-118">Not supported.</span></span>    |
|<span data-ttu-id="50833-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="50833-119">Application</span></span> | <span data-ttu-id="50833-120">AppRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="50833-120">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50833-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50833-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="50833-122">作为一种最佳做法，我们建议通过 `appRoleAssignedTo` _资源_服务主体的关系创建应用程序角色分配，而不是 `appRoleAssignments` 分配的用户、组或服务主体的关系。</span><span class="sxs-lookup"><span data-stu-id="50833-122">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50833-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="50833-123">Request headers</span></span>

| <span data-ttu-id="50833-124">名称</span><span class="sxs-lookup"><span data-stu-id="50833-124">Name</span></span>       | <span data-ttu-id="50833-125">说明</span><span class="sxs-lookup"><span data-stu-id="50833-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="50833-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="50833-126">Authorization</span></span> | <span data-ttu-id="50833-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50833-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50833-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50833-129">Content-Type</span></span> | <span data-ttu-id="50833-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="50833-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50833-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="50833-132">Request body</span></span>

<span data-ttu-id="50833-133">在请求正文中，提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50833-133">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="50833-134">响应</span><span class="sxs-lookup"><span data-stu-id="50833-134">Response</span></span>

<span data-ttu-id="50833-135">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="50833-135">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="50833-136">示例</span><span class="sxs-lookup"><span data-stu-id="50833-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="50833-137">请求</span><span class="sxs-lookup"><span data-stu-id="50833-137">Request</span></span>

<span data-ttu-id="50833-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50833-138">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="50833-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="50833-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/users/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="50833-140">C#</span><span class="sxs-lookup"><span data-stu-id="50833-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50833-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50833-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50833-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50833-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="50833-143">在此示例中， `{id}` 和 `{principalId-value}` 都是 `id` 分配的用户的。</span><span class="sxs-lookup"><span data-stu-id="50833-143">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned user.</span></span>

### <a name="response"></a><span data-ttu-id="50833-144">响应</span><span class="sxs-lookup"><span data-stu-id="50833-144">Response</span></span>

<span data-ttu-id="50833-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="50833-145">Here is an example of the response.</span></span> 

> <span data-ttu-id="50833-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="50833-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "id": "id-value",
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalType": "principalType-value",
  "principalId": "principalId-value",
  "principalDisplayName": "principalDisplayName-value",
  "resourceId": "resourceId-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
