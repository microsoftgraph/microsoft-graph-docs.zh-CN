---
title: case： close
description: 关闭电子数据展示案例。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d5fd2bcf997660dac803a9e417ee93d41f95882a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446103"
---
# <a name="case-close"></a><span data-ttu-id="a7d16-103">case： close</span><span class="sxs-lookup"><span data-stu-id="a7d16-103">case: close</span></span>

<span data-ttu-id="a7d16-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a7d16-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7d16-105">关闭电子数据展示案例。</span><span class="sxs-lookup"><span data-stu-id="a7d16-105">Close an eDiscovery case.</span></span> <span data-ttu-id="a7d16-106">有关详细信息，请参阅"[关闭案例"。](/microsoft-365/compliance/close-or-delete-case#close-a-case)</span><span class="sxs-lookup"><span data-stu-id="a7d16-106">For details, see [Close a case](/microsoft-365/compliance/close-or-delete-case#close-a-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7d16-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="a7d16-107">Permissions</span></span>

<span data-ttu-id="a7d16-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7d16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7d16-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7d16-110">Permission type</span></span>|<span data-ttu-id="a7d16-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7d16-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7d16-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7d16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7d16-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7d16-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a7d16-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7d16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7d16-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7d16-115">Not supported.</span></span>|
|<span data-ttu-id="a7d16-116">Application</span><span class="sxs-lookup"><span data-stu-id="a7d16-116">Application</span></span>|<span data-ttu-id="a7d16-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7d16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7d16-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7d16-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{CaseId}/close
```

## <a name="request-headers"></a><span data-ttu-id="a7d16-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7d16-119">Request headers</span></span>

|<span data-ttu-id="a7d16-120">名称</span><span class="sxs-lookup"><span data-stu-id="a7d16-120">Name</span></span>|<span data-ttu-id="a7d16-121">说明</span><span class="sxs-lookup"><span data-stu-id="a7d16-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a7d16-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7d16-122">Authorization</span></span>|<span data-ttu-id="a7d16-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7d16-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7d16-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7d16-125">Request body</span></span>

<span data-ttu-id="a7d16-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7d16-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7d16-127">响应</span><span class="sxs-lookup"><span data-stu-id="a7d16-127">Response</span></span>

<span data-ttu-id="a7d16-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a7d16-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a7d16-129">示例</span><span class="sxs-lookup"><span data-stu-id="a7d16-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a7d16-130">请求</span><span class="sxs-lookup"><span data-stu-id="a7d16-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a7d16-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7d16-131">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "case_close"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/close
```

# <a name="c"></a>[<span data-ttu-id="a7d16-132">C#</span><span class="sxs-lookup"><span data-stu-id="a7d16-132">C#</span></span>](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-close-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7d16-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7d16-133">JavaScript</span></span>](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-close-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7d16-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7d16-134">Objective-C</span></span>](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-close-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7d16-135">Java</span><span class="sxs-lookup"><span data-stu-id="a7d16-135">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-close-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="a7d16-136">响应</span><span class="sxs-lookup"><span data-stu-id="a7d16-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
