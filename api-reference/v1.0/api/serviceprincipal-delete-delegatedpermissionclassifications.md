---
title: 删除 delegatedPermissionClassification
description: 从 API 的服务主体中删除委派权限分类。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: decce0d0a9e3f6915676cb7151da0d43ddff3067
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133096"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="89157-103">删除 delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="89157-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="89157-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89157-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89157-105">删除以前为委派权限设置的[delegatedPermissionClassification。](../resources/delegatedPermissionClassification.md)</span><span class="sxs-lookup"><span data-stu-id="89157-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="89157-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="89157-106">Permissions</span></span>

<span data-ttu-id="89157-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89157-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="89157-109">Permission type</span></span>      | <span data-ttu-id="89157-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89157-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89157-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89157-111">Delegated (work or school account)</span></span> | <span data-ttu-id="89157-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89157-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="89157-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89157-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89157-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="89157-114">Not supported.</span></span>    |
|<span data-ttu-id="89157-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="89157-115">Application</span></span> | <span data-ttu-id="89157-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89157-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89157-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89157-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="89157-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="89157-118">Request headers</span></span>

| <span data-ttu-id="89157-119">名称</span><span class="sxs-lookup"><span data-stu-id="89157-119">Name</span></span>       | <span data-ttu-id="89157-120">类型</span><span class="sxs-lookup"><span data-stu-id="89157-120">Type</span></span> | <span data-ttu-id="89157-121">说明</span><span class="sxs-lookup"><span data-stu-id="89157-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89157-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89157-122">Authorization</span></span>  | <span data-ttu-id="89157-123">string</span><span class="sxs-lookup"><span data-stu-id="89157-123">string</span></span>  | <span data-ttu-id="89157-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89157-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89157-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="89157-126">Request body</span></span>

<span data-ttu-id="89157-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89157-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89157-128">响应</span><span class="sxs-lookup"><span data-stu-id="89157-128">Response</span></span>

<span data-ttu-id="89157-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="89157-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89157-131">示例</span><span class="sxs-lookup"><span data-stu-id="89157-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89157-132">请求</span><span class="sxs-lookup"><span data-stu-id="89157-132">Request</span></span>

<span data-ttu-id="89157-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89157-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="89157-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="89157-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="89157-135">C#</span><span class="sxs-lookup"><span data-stu-id="89157-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-delegatedpermissionclassifications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89157-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89157-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-delegatedpermissionclassifications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89157-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89157-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-delegatedpermissionclassifications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89157-138">Java</span><span class="sxs-lookup"><span data-stu-id="89157-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-delegatedpermissionclassifications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89157-139">响应</span><span class="sxs-lookup"><span data-stu-id="89157-139">Response</span></span>

<span data-ttu-id="89157-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="89157-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
