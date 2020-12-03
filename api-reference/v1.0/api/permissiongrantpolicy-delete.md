---
title: 删除 permissionGrantPolicy
description: 删除 permissionGrantPolicy 对象。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 45b91dd3480ba4228ed159b13dcaeeda2385c993
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524326"
---
# <a name="delete-permissiongrantpolicy"></a><span data-ttu-id="f52fa-103">删除 permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="f52fa-103">Delete permissionGrantPolicy</span></span>

<span data-ttu-id="f52fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f52fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f52fa-105">删除 [permissionGrantPolicy](../resources/permissiongrantpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f52fa-105">Delete a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f52fa-106">权限</span><span class="sxs-lookup"><span data-stu-id="f52fa-106">Permissions</span></span>

<span data-ttu-id="f52fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f52fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f52fa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f52fa-109">Permission type</span></span>                        | <span data-ttu-id="f52fa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f52fa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f52fa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f52fa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f52fa-112">PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f52fa-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="f52fa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f52fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f52fa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f52fa-114">Not supported.</span></span> |
| <span data-ttu-id="f52fa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f52fa-115">Application</span></span>                            | <span data-ttu-id="f52fa-116">PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f52fa-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="f52fa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f52fa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f52fa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f52fa-118">Request headers</span></span>

| <span data-ttu-id="f52fa-119">名称</span><span class="sxs-lookup"><span data-stu-id="f52fa-119">Name</span></span>           | <span data-ttu-id="f52fa-120">说明</span><span class="sxs-lookup"><span data-stu-id="f52fa-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f52fa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f52fa-121">Authorization</span></span>  | <span data-ttu-id="f52fa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f52fa-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f52fa-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f52fa-124">Request body</span></span>

<span data-ttu-id="f52fa-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f52fa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f52fa-126">响应</span><span class="sxs-lookup"><span data-stu-id="f52fa-126">Response</span></span>

<span data-ttu-id="f52fa-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f52fa-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f52fa-129">示例</span><span class="sxs-lookup"><span data-stu-id="f52fa-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f52fa-130">请求</span><span class="sxs-lookup"><span data-stu-id="f52fa-130">Request</span></span>

<span data-ttu-id="f52fa-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f52fa-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f52fa-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f52fa-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_permissiongrantpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy
```
# <a name="c"></a>[<span data-ttu-id="f52fa-133">C#</span><span class="sxs-lookup"><span data-stu-id="f52fa-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f52fa-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f52fa-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f52fa-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f52fa-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f52fa-136">Java</span><span class="sxs-lookup"><span data-stu-id="f52fa-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f52fa-137">响应</span><span class="sxs-lookup"><span data-stu-id="f52fa-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
