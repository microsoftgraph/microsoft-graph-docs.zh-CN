---
title: 从服务主体中删除 appRoleAssignment
description: 从服务主体中删除 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 4d573ef73aed7ebce12534c47797632eeb2ddb68
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458344"
---
# <a name="delete-an-approleassignment-granted-to-a-service-principal"></a><span data-ttu-id="4cee1-103">删除向服务主体授予的 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4cee1-103">Delete an appRoleAssignment granted to a service principal</span></span>

<span data-ttu-id="4cee1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cee1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cee1-105">删除已授予服务主体的 [appRoleAssignment](../resources/approleassignment.md) 。</span><span class="sxs-lookup"><span data-stu-id="4cee1-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a service principal has been granted.</span></span>

<span data-ttu-id="4cee1-106">分配给服务主体的应用程序角色也称为 " [应用程序权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)"。</span><span class="sxs-lookup"><span data-stu-id="4cee1-106">App roles which are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="4cee1-107">删除服务主体的应用程序角色分配等效于撤消仅应用权限授予。</span><span class="sxs-lookup"><span data-stu-id="4cee1-107">Deleting an app role assignment for a service principal is equivalent to revoking the app-only permission grant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cee1-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="4cee1-108">Permissions</span></span>

<span data-ttu-id="4cee1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4cee1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cee1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4cee1-111">Permission type</span></span>      | <span data-ttu-id="4cee1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4cee1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cee1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4cee1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4cee1-114">AppRoleAssignment.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4cee1-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4cee1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4cee1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cee1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cee1-116">Not supported.</span></span>    |
|<span data-ttu-id="4cee1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4cee1-117">Application</span></span> | <span data-ttu-id="4cee1-118">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cee1-118">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cee1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4cee1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="4cee1-120">作为一种最佳做法，我们建议通过 `appRoleAssignedTo` _资源_ 服务主体的关系（而不是 `appRoleAssignments` 分配的用户、组或服务主体的关系）删除应用程序角色分配。</span><span class="sxs-lookup"><span data-stu-id="4cee1-120">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cee1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4cee1-121">Request headers</span></span>

| <span data-ttu-id="4cee1-122">名称</span><span class="sxs-lookup"><span data-stu-id="4cee1-122">Name</span></span>       | <span data-ttu-id="4cee1-123">类型</span><span class="sxs-lookup"><span data-stu-id="4cee1-123">Type</span></span> | <span data-ttu-id="4cee1-124">说明</span><span class="sxs-lookup"><span data-stu-id="4cee1-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4cee1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cee1-125">Authorization</span></span>  | <span data-ttu-id="4cee1-126">string</span><span class="sxs-lookup"><span data-stu-id="4cee1-126">string</span></span>  | <span data-ttu-id="4cee1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4cee1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cee1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4cee1-129">Request body</span></span>

<span data-ttu-id="4cee1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4cee1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cee1-131">响应</span><span class="sxs-lookup"><span data-stu-id="4cee1-131">Response</span></span>

<span data-ttu-id="4cee1-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4cee1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4cee1-134">示例</span><span class="sxs-lookup"><span data-stu-id="4cee1-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4cee1-135">请求</span><span class="sxs-lookup"><span data-stu-id="4cee1-135">Request</span></span>

<span data-ttu-id="4cee1-136">下面的示例展示了删除应用程序角色分配的请求。</span><span class="sxs-lookup"><span data-stu-id="4cee1-136">Here is an example of the request to delete an app role assignment.</span></span>


# <a name="http"></a>[<span data-ttu-id="4cee1-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cee1-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="4cee1-138">C#</span><span class="sxs-lookup"><span data-stu-id="4cee1-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4cee1-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cee1-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4cee1-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4cee1-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4cee1-141">Java</span><span class="sxs-lookup"><span data-stu-id="4cee1-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-approleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4cee1-142">响应</span><span class="sxs-lookup"><span data-stu-id="4cee1-142">Response</span></span>

<span data-ttu-id="4cee1-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4cee1-143">The following is an example of the response.</span></span>

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
