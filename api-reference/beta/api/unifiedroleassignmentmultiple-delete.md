---
title: 删除 unifiedRoleAssignmentMultiple
description: 删除 unifiedRoleAssignmentMultiple 对象。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2d253c5e214887eed33481673d81c47e1c305e3c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004298"
---
# <a name="delete-unifiedroleassignmentmultiple"></a><span data-ttu-id="0bbd4-103">删除 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="0bbd4-103">Delete unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="0bbd4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bbd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bbd4-105">删除 [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0bbd4-105">Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="0bbd4-106">这适用于支持多个主体和作用域的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="0bbd4-106">This is applicable for a RBAC application that supports multiple principals and scopes.</span></span> <span data-ttu-id="0bbd4-107">Microsoft Intune 是这样一个应用程序。</span><span class="sxs-lookup"><span data-stu-id="0bbd4-107">Microsoft Intune is such an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bbd4-108">权限</span><span class="sxs-lookup"><span data-stu-id="0bbd4-108">Permissions</span></span>

<span data-ttu-id="0bbd4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0bbd4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0bbd4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bbd4-111">Permission type</span></span> | <span data-ttu-id="0bbd4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0bbd4-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="0bbd4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bbd4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0bbd4-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bbd4-114">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="0bbd4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bbd4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bbd4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bbd4-116">Not supported.</span></span> |
| <span data-ttu-id="0bbd4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bbd4-117">Application</span></span> | <span data-ttu-id="0bbd4-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bbd4-118">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bbd4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bbd4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0bbd4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bbd4-120">Request headers</span></span>

| <span data-ttu-id="0bbd4-121">名称</span><span class="sxs-lookup"><span data-stu-id="0bbd4-121">Name</span></span> | <span data-ttu-id="0bbd4-122">说明</span><span class="sxs-lookup"><span data-stu-id="0bbd4-122">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="0bbd4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bbd4-123">Authorization</span></span> | <span data-ttu-id="0bbd4-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0bbd4-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0bbd4-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bbd4-125">Request body</span></span>

<span data-ttu-id="0bbd4-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0bbd4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bbd4-127">响应</span><span class="sxs-lookup"><span data-stu-id="0bbd4-127">Response</span></span>

<span data-ttu-id="0bbd4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0bbd4-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bbd4-130">示例</span><span class="sxs-lookup"><span data-stu-id="0bbd4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bbd4-131">请求</span><span class="sxs-lookup"><span data-stu-id="0bbd4-131">Request</span></span>

<span data-ttu-id="0bbd4-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0bbd4-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0bbd4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0bbd4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignmentMultiple"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="0bbd4-134">C#</span><span class="sxs-lookup"><span data-stu-id="0bbd4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0bbd4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bbd4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0bbd4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0bbd4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0bbd4-137">响应</span><span class="sxs-lookup"><span data-stu-id="0bbd4-137">Response</span></span>

<span data-ttu-id="0bbd4-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0bbd4-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


