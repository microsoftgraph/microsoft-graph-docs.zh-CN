---
title: 删除 userSource
description: 删除 userSource 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 86792f5fe7375d3abc644d718f0bf22c96e1f147
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445975"
---
# <a name="delete-usersource"></a><span data-ttu-id="a181b-103">删除 userSource</span><span class="sxs-lookup"><span data-stu-id="a181b-103">Delete userSource</span></span>

<span data-ttu-id="a181b-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a181b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a181b-105">删除 [userSource](../resources/ediscovery-usersource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a181b-105">Delete a [userSource](../resources/ediscovery-usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a181b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a181b-106">Permissions</span></span>

<span data-ttu-id="a181b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a181b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a181b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a181b-109">Permission type</span></span>|<span data-ttu-id="a181b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a181b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a181b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a181b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a181b-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a181b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a181b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a181b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a181b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a181b-114">Not supported.</span></span>|
|<span data-ttu-id="a181b-115">Application</span><span class="sxs-lookup"><span data-stu-id="a181b-115">Application</span></span>|<span data-ttu-id="a181b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a181b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a181b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a181b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="a181b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a181b-118">Request headers</span></span>

|<span data-ttu-id="a181b-119">名称</span><span class="sxs-lookup"><span data-stu-id="a181b-119">Name</span></span>|<span data-ttu-id="a181b-120">说明</span><span class="sxs-lookup"><span data-stu-id="a181b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a181b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a181b-121">Authorization</span></span>|<span data-ttu-id="a181b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a181b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a181b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a181b-124">Request body</span></span>

<span data-ttu-id="a181b-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a181b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a181b-126">响应</span><span class="sxs-lookup"><span data-stu-id="a181b-126">Response</span></span>

<span data-ttu-id="a181b-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a181b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a181b-128">示例</span><span class="sxs-lookup"><span data-stu-id="a181b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a181b-129">请求</span><span class="sxs-lookup"><span data-stu-id="a181b-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a181b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a181b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_usersource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```
# <a name="c"></a>[<span data-ttu-id="a181b-131">C#</span><span class="sxs-lookup"><span data-stu-id="a181b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a181b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a181b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a181b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a181b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a181b-134">Java</span><span class="sxs-lookup"><span data-stu-id="a181b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a181b-135">响应</span><span class="sxs-lookup"><span data-stu-id="a181b-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
