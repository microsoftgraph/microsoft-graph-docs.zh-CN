---
title: 删除为服务主体授予的 appRoleAssignment
description: 删除为服务主体授予的 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: bf1f30f336347bbac1bf5903c8275de773c32532
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870568"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="83e18-103">删除为服务主体授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="83e18-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="83e18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83e18-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83e18-105">删除已授予资源服务主体的用户、组或客户端服务主体的[appRoleAssignment。](../resources/approleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="83e18-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="83e18-106">权限</span><span class="sxs-lookup"><span data-stu-id="83e18-106">Permissions</span></span>

<span data-ttu-id="83e18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83e18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83e18-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83e18-109">Permission type</span></span>      | <span data-ttu-id="83e18-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83e18-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83e18-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83e18-111">Delegated (work or school account)</span></span> | <span data-ttu-id="83e18-112">AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="83e18-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="83e18-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83e18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83e18-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83e18-114">Not supported.</span></span>    |
|<span data-ttu-id="83e18-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83e18-115">Application</span></span> | <span data-ttu-id="83e18-116">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83e18-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83e18-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83e18-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{principal-id}
```

> [!NOTE]
> <span data-ttu-id="83e18-118">作为最佳实践，我们建议通过资源服务主体的关系（而不是分配的用户、组或服务主体的关系）删除应用程序 `appRoleAssignedTo`  `appRoleAssignments` 角色分配。</span><span class="sxs-lookup"><span data-stu-id="83e18-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="83e18-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="83e18-119">Request headers</span></span>

| <span data-ttu-id="83e18-120">名称</span><span class="sxs-lookup"><span data-stu-id="83e18-120">Name</span></span>       | <span data-ttu-id="83e18-121">类型</span><span class="sxs-lookup"><span data-stu-id="83e18-121">Type</span></span> | <span data-ttu-id="83e18-122">说明</span><span class="sxs-lookup"><span data-stu-id="83e18-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="83e18-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83e18-123">Authorization</span></span>  | <span data-ttu-id="83e18-124">string</span><span class="sxs-lookup"><span data-stu-id="83e18-124">string</span></span>  | <span data-ttu-id="83e18-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83e18-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83e18-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="83e18-127">Request body</span></span>

<span data-ttu-id="83e18-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="83e18-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83e18-129">响应</span><span class="sxs-lookup"><span data-stu-id="83e18-129">Response</span></span>

<span data-ttu-id="83e18-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="83e18-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83e18-132">示例</span><span class="sxs-lookup"><span data-stu-id="83e18-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83e18-133">请求</span><span class="sxs-lookup"><span data-stu-id="83e18-133">Request</span></span>

<span data-ttu-id="83e18-134">下面是从资源服务主体角色分配应用程序请求的示例。</span><span class="sxs-lookup"><span data-stu-id="83e18-134">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="83e18-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="83e18-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{principalId}
```
# <a name="c"></a>[<span data-ttu-id="83e18-136">C#</span><span class="sxs-lookup"><span data-stu-id="83e18-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83e18-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83e18-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83e18-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83e18-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83e18-139">Java</span><span class="sxs-lookup"><span data-stu-id="83e18-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="83e18-140">此示例中， 将是资源服务主体的 ID，并且将是分配的用户、组或客户端 `{resource-SP-id}` `{principalId}` 服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="83e18-140">In this example, `{resource-SP-id}` would be the id of the resource service principal, and `{principalId}` would be the id of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="83e18-141">响应</span><span class="sxs-lookup"><span data-stu-id="83e18-141">Response</span></span>

<span data-ttu-id="83e18-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="83e18-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

