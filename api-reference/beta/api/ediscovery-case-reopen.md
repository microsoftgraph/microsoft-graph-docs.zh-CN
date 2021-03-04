---
title: case： reopen
description: 重新打开已关闭的电子数据展示案例。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5eaa03b81502273e6aae914fa699311457df9cd9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446075"
---
# <a name="case-reopen"></a><span data-ttu-id="0ee46-103">case： reopen</span><span class="sxs-lookup"><span data-stu-id="0ee46-103">case: reopen</span></span>

<span data-ttu-id="0ee46-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="0ee46-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ee46-105">重新打开已关闭的电子数据展示案例。</span><span class="sxs-lookup"><span data-stu-id="0ee46-105">Reopen an eDiscovery case that was closed.</span></span> <span data-ttu-id="0ee46-106">有关详细信息，请参阅重新打开 [已关闭的大小写](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case)。</span><span class="sxs-lookup"><span data-stu-id="0ee46-106">For details, see [Reopen a closed case](/microsoft-365/compliance/close-or-delete-case#reopen-a-closed-case).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ee46-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="0ee46-107">Permissions</span></span>

<span data-ttu-id="0ee46-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ee46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee46-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ee46-110">Permission type</span></span>|<span data-ttu-id="0ee46-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ee46-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee46-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ee46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee46-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee46-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="0ee46-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ee46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee46-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ee46-115">Not supported.</span></span>|
|<span data-ttu-id="0ee46-116">Application</span><span class="sxs-lookup"><span data-stu-id="0ee46-116">Application</span></span>|<span data-ttu-id="0ee46-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ee46-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee46-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ee46-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/reopen
```

## <a name="request-headers"></a><span data-ttu-id="0ee46-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ee46-119">Request headers</span></span>

|<span data-ttu-id="0ee46-120">名称</span><span class="sxs-lookup"><span data-stu-id="0ee46-120">Name</span></span>|<span data-ttu-id="0ee46-121">说明</span><span class="sxs-lookup"><span data-stu-id="0ee46-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0ee46-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ee46-122">Authorization</span></span>|<span data-ttu-id="0ee46-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ee46-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee46-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ee46-125">Request body</span></span>

<span data-ttu-id="0ee46-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ee46-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ee46-127">响应</span><span class="sxs-lookup"><span data-stu-id="0ee46-127">Response</span></span>

<span data-ttu-id="0ee46-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0ee46-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0ee46-129">示例</span><span class="sxs-lookup"><span data-stu-id="0ee46-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ee46-130">请求</span><span class="sxs-lookup"><span data-stu-id="0ee46-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0ee46-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ee46-131">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "case_reopen"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/reopen
```
# <a name="c"></a>[<span data-ttu-id="0ee46-132">C#</span><span class="sxs-lookup"><span data-stu-id="0ee46-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycase-reopen-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ee46-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ee46-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycase-reopen-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ee46-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ee46-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/ediscoverycase-reopen-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ee46-135">Java</span><span class="sxs-lookup"><span data-stu-id="0ee46-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycase-reopen-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0ee46-136">响应</span><span class="sxs-lookup"><span data-stu-id="0ee46-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
