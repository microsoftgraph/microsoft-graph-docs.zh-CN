---
title: noncustodialDataSource：release
description: 从用例中释放非安全数据源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 190845ea64a545b29c2de60028ca22746ba8b91f
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316956"
---
# <a name="noncustodialdatasource-release"></a><span data-ttu-id="7175d-103">noncustodialDataSource：release</span><span class="sxs-lookup"><span data-stu-id="7175d-103">noncustodialDataSource: release</span></span>

<span data-ttu-id="7175d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7175d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7175d-105">从用例中释放非安全数据源。</span><span class="sxs-lookup"><span data-stu-id="7175d-105">Releases the non-custodial data source from the case.</span></span>

## <a name="permissions"></a><span data-ttu-id="7175d-106">权限</span><span class="sxs-lookup"><span data-stu-id="7175d-106">Permissions</span></span>

<span data-ttu-id="7175d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7175d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7175d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7175d-109">Permission type</span></span>|<span data-ttu-id="7175d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7175d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7175d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7175d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7175d-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7175d-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="7175d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7175d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7175d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7175d-114">Not supported.</span></span>|
|<span data-ttu-id="7175d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7175d-115">Application</span></span>|<span data-ttu-id="7175d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7175d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7175d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7175d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}/release
```

## <a name="request-headers"></a><span data-ttu-id="7175d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7175d-118">Request headers</span></span>

|<span data-ttu-id="7175d-119">名称</span><span class="sxs-lookup"><span data-stu-id="7175d-119">Name</span></span>|<span data-ttu-id="7175d-120">说明</span><span class="sxs-lookup"><span data-stu-id="7175d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7175d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7175d-121">Authorization</span></span>|<span data-ttu-id="7175d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7175d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7175d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7175d-124">Request body</span></span>

<span data-ttu-id="7175d-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7175d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7175d-126">响应</span><span class="sxs-lookup"><span data-stu-id="7175d-126">Response</span></span>

<span data-ttu-id="7175d-127">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7175d-127">If successful, this action returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7175d-128">示例</span><span class="sxs-lookup"><span data-stu-id="7175d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7175d-129">请求</span><span class="sxs-lookup"><span data-stu-id="7175d-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7175d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7175d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "noncustodialdatasource_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/release
```
# <a name="c"></a>[<span data-ttu-id="7175d-131">C#</span><span class="sxs-lookup"><span data-stu-id="7175d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/noncustodialdatasource-release-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7175d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7175d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/noncustodialdatasource-release-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7175d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7175d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/noncustodialdatasource-release-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7175d-134">Java</span><span class="sxs-lookup"><span data-stu-id="7175d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/noncustodialdatasource-release-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7175d-135">响应</span><span class="sxs-lookup"><span data-stu-id="7175d-135">Response</span></span>

<span data-ttu-id="7175d-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7175d-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```
