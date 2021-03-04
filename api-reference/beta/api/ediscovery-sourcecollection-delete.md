---
title: 删除 sourceCollection
description: 删除 sourceCollection 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 38debc57e715b735e56be154f57bbef8861cae05
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446013"
---
# <a name="delete-sourcecollection"></a><span data-ttu-id="f949e-103">删除 sourceCollection</span><span class="sxs-lookup"><span data-stu-id="f949e-103">Delete sourceCollection</span></span>

<span data-ttu-id="f949e-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f949e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f949e-105">删除 [sourceCollection](../resources/ediscovery-sourcecollection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f949e-105">Delete a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f949e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f949e-106">Permissions</span></span>

<span data-ttu-id="f949e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f949e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f949e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f949e-109">Permission type</span></span>|<span data-ttu-id="f949e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f949e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f949e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f949e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f949e-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f949e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f949e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f949e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f949e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f949e-114">Not supported.</span></span>|
|<span data-ttu-id="f949e-115">Application</span><span class="sxs-lookup"><span data-stu-id="f949e-115">Application</span></span>|<span data-ttu-id="f949e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f949e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f949e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f949e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="request-headers"></a><span data-ttu-id="f949e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f949e-118">Request headers</span></span>

|<span data-ttu-id="f949e-119">名称</span><span class="sxs-lookup"><span data-stu-id="f949e-119">Name</span></span>|<span data-ttu-id="f949e-120">说明</span><span class="sxs-lookup"><span data-stu-id="f949e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f949e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f949e-121">Authorization</span></span>|<span data-ttu-id="f949e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f949e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f949e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f949e-124">Request body</span></span>

<span data-ttu-id="f949e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f949e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f949e-126">响应</span><span class="sxs-lookup"><span data-stu-id="f949e-126">Response</span></span>

<span data-ttu-id="f949e-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f949e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f949e-128">示例</span><span class="sxs-lookup"><span data-stu-id="f949e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f949e-129">请求</span><span class="sxs-lookup"><span data-stu-id="f949e-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_sourcecollection"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

### <a name="response"></a><span data-ttu-id="f949e-130">响应</span><span class="sxs-lookup"><span data-stu-id="f949e-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
