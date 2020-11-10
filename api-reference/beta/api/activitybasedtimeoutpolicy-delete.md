---
title: 删除 activityBasedTimeoutPolicy
description: 删除 activityBasedTimeoutPolicy。
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b874e5e7625df1e61ef0e289624bfe441094ee0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952569"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="6d132-103">删除 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="6d132-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="6d132-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d132-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d132-105">删除 [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d132-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d132-106">权限</span><span class="sxs-lookup"><span data-stu-id="6d132-106">Permissions</span></span>

<span data-ttu-id="6d132-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d132-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d132-109">Permission type</span></span>                        | <span data-ttu-id="6d132-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d132-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6d132-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d132-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d132-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d132-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6d132-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d132-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d132-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d132-114">Not supported.</span></span> |
| <span data-ttu-id="6d132-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d132-115">Application</span></span>                            | <span data-ttu-id="6d132-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d132-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d132-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d132-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6d132-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d132-118">Request headers</span></span>

| <span data-ttu-id="6d132-119">名称</span><span class="sxs-lookup"><span data-stu-id="6d132-119">Name</span></span>          | <span data-ttu-id="6d132-120">说明</span><span class="sxs-lookup"><span data-stu-id="6d132-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6d132-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d132-121">Authorization</span></span> | <span data-ttu-id="6d132-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="6d132-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d132-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d132-123">Request body</span></span>

<span data-ttu-id="6d132-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6d132-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d132-125">响应</span><span class="sxs-lookup"><span data-stu-id="6d132-125">Response</span></span>

<span data-ttu-id="6d132-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6d132-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6d132-127">示例</span><span class="sxs-lookup"><span data-stu-id="6d132-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d132-128">请求</span><span class="sxs-lookup"><span data-stu-id="6d132-128">Request</span></span>

<span data-ttu-id="6d132-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6d132-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6d132-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d132-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="6d132-131">C#</span><span class="sxs-lookup"><span data-stu-id="6d132-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d132-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d132-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d132-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d132-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d132-134">Java</span><span class="sxs-lookup"><span data-stu-id="6d132-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6d132-135">响应</span><span class="sxs-lookup"><span data-stu-id="6d132-135">Response</span></span>

<span data-ttu-id="6d132-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6d132-136">The following is an example of the response.</span></span>

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
  "description": "Delete activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


