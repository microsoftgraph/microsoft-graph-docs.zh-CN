---
title: 向用户授予 appRoleAssignment
description: 向用户授予应用角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 9c0df54ed9a4d6a5079f2c6ce587793d6d8a3982
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135938"
---
# <a name="grant-an-approleassignment-to-a-user"></a><span data-ttu-id="50b70-103">向用户授予 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="50b70-103">Grant an appRoleAssignment to a user</span></span>

<span data-ttu-id="50b70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50b70-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50b70-105">使用此 API 将应用角色分配给用户。</span><span class="sxs-lookup"><span data-stu-id="50b70-105">Use this API to assign an app role to a user.</span></span> <span data-ttu-id="50b70-106">若要向用户授予应用角色分配，需使用三个标识符：</span><span class="sxs-lookup"><span data-stu-id="50b70-106">To grant an app role assignment to a user, you need three identifiers:</span></span>

- <span data-ttu-id="50b70-107">`principalId`：要向其分配应用角色的用户的 `id`。</span><span class="sxs-lookup"><span data-stu-id="50b70-107">`principalId`: The `id` of the user to whom you are assigning the app role.</span></span>
- <span data-ttu-id="50b70-108">`resourceId`：已定义应用角色的资源 `servicePrincipal` 的 `id`。</span><span class="sxs-lookup"><span data-stu-id="50b70-108">`resourceId`: The `id` of the resource `servicePrincipal` that has defined the app role.</span></span>
- <span data-ttu-id="50b70-109">`appRoleId`：要分配给用户的 `appRole`（在资源服务主体上定义）的 `id`。</span><span class="sxs-lookup"><span data-stu-id="50b70-109">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="50b70-110">权限</span><span class="sxs-lookup"><span data-stu-id="50b70-110">Permissions</span></span>

<span data-ttu-id="50b70-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50b70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50b70-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="50b70-113">Permission type</span></span>      | <span data-ttu-id="50b70-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50b70-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50b70-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50b70-115">Delegated (work or school account)</span></span> | <span data-ttu-id="50b70-116">AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50b70-116">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50b70-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50b70-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50b70-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="50b70-118">Not supported.</span></span>    |
|<span data-ttu-id="50b70-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="50b70-119">Application</span></span> | <span data-ttu-id="50b70-120">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b70-120">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50b70-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50b70-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="50b70-122">最佳做法是，建议通过 _资源_ 服务主体的 `appRoleAssignedTo` 关系（而不是通过分配的用户、组或服务主体的 `appRoleAssignments` 关系）创建应用角色分配。</span><span class="sxs-lookup"><span data-stu-id="50b70-122">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50b70-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="50b70-123">Request headers</span></span>

| <span data-ttu-id="50b70-124">名称</span><span class="sxs-lookup"><span data-stu-id="50b70-124">Name</span></span>       | <span data-ttu-id="50b70-125">说明</span><span class="sxs-lookup"><span data-stu-id="50b70-125">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="50b70-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="50b70-126">Authorization</span></span> | <span data-ttu-id="50b70-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50b70-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50b70-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50b70-129">Content-Type</span></span> | <span data-ttu-id="50b70-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="50b70-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50b70-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="50b70-132">Request body</span></span>

<span data-ttu-id="50b70-133">在请求正文中，提供 [appRoleAssignment](../resources/approleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50b70-133">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="50b70-134">响应</span><span class="sxs-lookup"><span data-stu-id="50b70-134">Response</span></span>

<span data-ttu-id="50b70-135">如果成功，此运营商将在响应正文中返回 `201 Created` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50b70-135">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="50b70-136">示例</span><span class="sxs-lookup"><span data-stu-id="50b70-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="50b70-137">请求</span><span class="sxs-lookup"><span data-stu-id="50b70-137">Request</span></span>

<span data-ttu-id="50b70-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50b70-138">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="50b70-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="50b70-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/v1.0/users/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="50b70-140">C#</span><span class="sxs-lookup"><span data-stu-id="50b70-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-create-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50b70-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50b70-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-create-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50b70-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50b70-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-create-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50b70-143">Java</span><span class="sxs-lookup"><span data-stu-id="50b70-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-create-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="50b70-144">在此示例中，`{id}` 和 `{principalId-value}` 均为已分配用户的 `id`。</span><span class="sxs-lookup"><span data-stu-id="50b70-144">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned user.</span></span>

### <a name="response"></a><span data-ttu-id="50b70-145">响应</span><span class="sxs-lookup"><span data-stu-id="50b70-145">Response</span></span>

<span data-ttu-id="50b70-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="50b70-146">Here is an example of the response.</span></span> 

> <span data-ttu-id="50b70-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="50b70-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

