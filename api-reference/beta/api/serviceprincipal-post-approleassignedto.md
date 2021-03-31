---
title: 为服务主体授予 appRoleAssignment
description: 为服务主体授予应用角色分配。
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 82b037e9a5dfd578d9df473873a551383d9546bd
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468672"
---
# <a name="grant-an-approleassignment-for-a-service-principal"></a><span data-ttu-id="849d7-103">为服务主体授予 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="849d7-103">Grant an appRoleAssignment for a service principal</span></span>

<span data-ttu-id="849d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="849d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="849d7-105">将资源服务主体的应用角色，分配给用户、组或客户端服务主体。</span><span class="sxs-lookup"><span data-stu-id="849d7-105">Assign an app role for a resource service principal, to a user, group, or client service principal.</span></span>

<span data-ttu-id="849d7-106">分配给服务主体的应用角色也被称为[应用程序权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)。</span><span class="sxs-lookup"><span data-stu-id="849d7-106">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="849d7-107">应用程序权限可以通过应用角色分配直接授予，或通过[协议体验](/azure/active-directory/develop/application-consent-experience)授予。</span><span class="sxs-lookup"><span data-stu-id="849d7-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="849d7-108">若要授予应用角色分配，需使用三个标识符：</span><span class="sxs-lookup"><span data-stu-id="849d7-108">To grant an app role assignment, you need three identifiers:</span></span>

- <span data-ttu-id="849d7-109">`principalId`： **用户** 的 `id`，**组** 或要向其分配应用程序角色的客户端 **servicePrincipal**。</span><span class="sxs-lookup"><span data-stu-id="849d7-109">`principalId`: The `id` of the **user**, **group** or client **servicePrincipal** to which you are assigning the app role.</span></span>
- <span data-ttu-id="849d7-110">`resourceId`：已定义应用角色的资源 **servicePrincipal** 的 `id`。</span><span class="sxs-lookup"><span data-stu-id="849d7-110">`resourceId`: The `id` of the resource **servicePrincipal** which has defined the app role.</span></span>
- <span data-ttu-id="849d7-111">`appRoleId`： **appRole** 中的 `id`来分配给用户、组或服务主体。</span><span class="sxs-lookup"><span data-stu-id="849d7-111">`appRoleId`: The `id` of the **appRole** (defined on the resource service principal) to assign to a user, group, or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="849d7-112">权限</span><span class="sxs-lookup"><span data-stu-id="849d7-112">Permissions</span></span>

<span data-ttu-id="849d7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="849d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="849d7-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="849d7-115">Permission type</span></span>      | <span data-ttu-id="849d7-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="849d7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="849d7-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="849d7-117">Delegated (work or school account)</span></span> | <span data-ttu-id="849d7-118">AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="849d7-118">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="849d7-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="849d7-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="849d7-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="849d7-120">Not supported.</span></span>    |
|<span data-ttu-id="849d7-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="849d7-121">Application</span></span> | <span data-ttu-id="849d7-122">AppRoleAssignment.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="849d7-122">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="849d7-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="849d7-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="request-headers"></a><span data-ttu-id="849d7-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="849d7-124">Request headers</span></span>

| <span data-ttu-id="849d7-125">名称</span><span class="sxs-lookup"><span data-stu-id="849d7-125">Name</span></span>       | <span data-ttu-id="849d7-126">说明</span><span class="sxs-lookup"><span data-stu-id="849d7-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="849d7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="849d7-127">Authorization</span></span> | <span data-ttu-id="849d7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="849d7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="849d7-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="849d7-130">Content-type</span></span> | <span data-ttu-id="849d7-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="849d7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="849d7-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="849d7-133">Request body</span></span>

<span data-ttu-id="849d7-134">在请求正文中，提供 [appRoleAssignment](../resources/approleassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="849d7-134">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="849d7-135">响应</span><span class="sxs-lookup"><span data-stu-id="849d7-135">Response</span></span>

<span data-ttu-id="849d7-136">如果成功，此运营商将在响应正文中返回 `201 Created` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="849d7-136">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="849d7-137">示例</span><span class="sxs-lookup"><span data-stu-id="849d7-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="849d7-138">请求</span><span class="sxs-lookup"><span data-stu-id="849d7-138">Request</span></span>

<span data-ttu-id="849d7-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="849d7-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="849d7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="849d7-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_approleassignedto"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/9028d19c-26a9-4809-8e3f-20ff73e2d75e/appRoleAssignedTo
Content-Type: application/json

{
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e",
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7"
}
```
# <a name="c"></a>[<span data-ttu-id="849d7-141">C#</span><span class="sxs-lookup"><span data-stu-id="849d7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-create-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="849d7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="849d7-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-create-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="849d7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="849d7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-create-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="849d7-144">Java</span><span class="sxs-lookup"><span data-stu-id="849d7-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-create-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="849d7-145">在此示例中，`{id}` 和 `{resourceId-value}` 是资源服务主体的 `id`，`{principalId}` 是分配的用户、组或客户端服务主体的 `id`。</span><span class="sxs-lookup"><span data-stu-id="849d7-145">In this example, `{id}` and `{resourceId-value}` would both be the `id` of the resource service principal, and `{principalId}` would be the `id` of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="849d7-146">响应</span><span class="sxs-lookup"><span data-stu-id="849d7-146">Response</span></span>

<span data-ttu-id="849d7-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="849d7-147">Here is an example of the response.</span></span> 

> <span data-ttu-id="849d7-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="849d7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('9028d19c-26a9-4809-8e3f-20ff73e2d75e')/appRoleAssignedTo/$entity",
  "id": "-WmtM5na7Uus0D8kI1yylpU9Mdo0Pb9OoBJvd3T5eKc",
  "deletedDateTime": null,
  "appRoleId": "ef7437e6-4f94-4a0a-a110-a439eb2aa8f7",
  "creationTimestamp": "2021-02-15T16:14:59.8643039Z",
  "principalDisplayName": "Parents of Contoso",
  "principalId": "33ad69f9-da99-4bed-acd0-3f24235cb296",
  "principalType": "Group",
  "resourceDisplayName": "Fabrikam App",
  "resourceId": "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
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
