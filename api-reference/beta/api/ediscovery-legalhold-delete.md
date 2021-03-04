---
title: 删除 legalHold
description: 删除 legalHold 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 90a7600f972a08220579dec56b1e0f738459c283
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446045"
---
# <a name="delete-legalhold"></a><span data-ttu-id="5a3bf-103">删除 legalHold</span><span class="sxs-lookup"><span data-stu-id="5a3bf-103">Delete legalHold</span></span>

<span data-ttu-id="5a3bf-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="5a3bf-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a3bf-105">删除 [legalHold](../resources/ediscovery-legalhold.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a3bf-105">Delete a [legalHold](../resources/ediscovery-legalhold.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a3bf-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5a3bf-106">Permissions</span></span>

<span data-ttu-id="5a3bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a3bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a3bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a3bf-109">Permission type</span></span>|<span data-ttu-id="5a3bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a3bf-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a3bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a3bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5a3bf-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a3bf-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="5a3bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a3bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a3bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a3bf-114">Not supported.</span></span>|
|<span data-ttu-id="5a3bf-115">Application</span><span class="sxs-lookup"><span data-stu-id="5a3bf-115">Application</span></span>|<span data-ttu-id="5a3bf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a3bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a3bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a3bf-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/legalHolds/{legalHoldId}
```

## <a name="request-headers"></a><span data-ttu-id="5a3bf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a3bf-118">Request headers</span></span>

|<span data-ttu-id="5a3bf-119">名称</span><span class="sxs-lookup"><span data-stu-id="5a3bf-119">Name</span></span>|<span data-ttu-id="5a3bf-120">说明</span><span class="sxs-lookup"><span data-stu-id="5a3bf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5a3bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a3bf-121">Authorization</span></span>|<span data-ttu-id="5a3bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a3bf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a3bf-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a3bf-124">Request body</span></span>

<span data-ttu-id="5a3bf-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5a3bf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a3bf-126">响应</span><span class="sxs-lookup"><span data-stu-id="5a3bf-126">Response</span></span>

<span data-ttu-id="5a3bf-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5a3bf-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5a3bf-128">示例</span><span class="sxs-lookup"><span data-stu-id="5a3bf-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a3bf-129">请求</span><span class="sxs-lookup"><span data-stu-id="5a3bf-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_legalhold"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}
```

### <a name="response"></a><span data-ttu-id="5a3bf-130">响应</span><span class="sxs-lookup"><span data-stu-id="5a3bf-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
