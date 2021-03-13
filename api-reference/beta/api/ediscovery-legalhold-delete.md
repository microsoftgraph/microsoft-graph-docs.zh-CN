---
title: 删除 legalHold
description: 删除 legalHold 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 84d94cf4ce0d340d36cb0cf5f2b478c70581f374
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773128"
---
# <a name="delete-legalhold"></a><span data-ttu-id="25d1f-103">删除 legalHold</span><span class="sxs-lookup"><span data-stu-id="25d1f-103">Delete legalHold</span></span>

<span data-ttu-id="25d1f-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="25d1f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25d1f-105">删除 [legalHold](../resources/ediscovery-legalhold.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="25d1f-105">Delete a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="25d1f-106">权限</span><span class="sxs-lookup"><span data-stu-id="25d1f-106">Permissions</span></span>

<span data-ttu-id="25d1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25d1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25d1f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="25d1f-109">Permission type</span></span>|<span data-ttu-id="25d1f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25d1f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25d1f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25d1f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="25d1f-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25d1f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="25d1f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25d1f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25d1f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="25d1f-114">Not supported.</span></span>|
|<span data-ttu-id="25d1f-115">Application</span><span class="sxs-lookup"><span data-stu-id="25d1f-115">Application</span></span>|<span data-ttu-id="25d1f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="25d1f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25d1f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25d1f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/legalHolds/{legalHoldId}
```

## <a name="request-headers"></a><span data-ttu-id="25d1f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="25d1f-118">Request headers</span></span>

|<span data-ttu-id="25d1f-119">名称</span><span class="sxs-lookup"><span data-stu-id="25d1f-119">Name</span></span>|<span data-ttu-id="25d1f-120">说明</span><span class="sxs-lookup"><span data-stu-id="25d1f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="25d1f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="25d1f-121">Authorization</span></span>|<span data-ttu-id="25d1f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="25d1f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="25d1f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="25d1f-124">Request body</span></span>

<span data-ttu-id="25d1f-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="25d1f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25d1f-126">响应</span><span class="sxs-lookup"><span data-stu-id="25d1f-126">Response</span></span>

<span data-ttu-id="25d1f-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="25d1f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="25d1f-128">示例</span><span class="sxs-lookup"><span data-stu-id="25d1f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25d1f-129">请求</span><span class="sxs-lookup"><span data-stu-id="25d1f-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="25d1f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="25d1f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_legalhold"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```
# <a name="c"></a>[<span data-ttu-id="25d1f-131">C#</span><span class="sxs-lookup"><span data-stu-id="25d1f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-legalhold-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25d1f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25d1f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-legalhold-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25d1f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25d1f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-legalhold-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25d1f-134">Java</span><span class="sxs-lookup"><span data-stu-id="25d1f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-legalhold-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="25d1f-135">响应</span><span class="sxs-lookup"><span data-stu-id="25d1f-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
