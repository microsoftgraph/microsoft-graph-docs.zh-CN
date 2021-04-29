---
title: noncustodialDataSource：Release
description: 从用例中释放非安全数据源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 9907ad3222af084cd349585f27df0a71221b22e6
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080725"
---
# <a name="noncustodialdatasource-release"></a><span data-ttu-id="e95c5-103">noncustodialDataSource：release</span><span class="sxs-lookup"><span data-stu-id="e95c5-103">noncustodialDataSource: release</span></span>

<span data-ttu-id="e95c5-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e95c5-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e95c5-105">从用例中释放非安全数据源。</span><span class="sxs-lookup"><span data-stu-id="e95c5-105">Releases the non-custodial data source from the case.</span></span>

## <a name="permissions"></a><span data-ttu-id="e95c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="e95c5-106">Permissions</span></span>

<span data-ttu-id="e95c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e95c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e95c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e95c5-109">Permission type</span></span>|<span data-ttu-id="e95c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e95c5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e95c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e95c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e95c5-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e95c5-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e95c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e95c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e95c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e95c5-114">Not supported.</span></span>|
|<span data-ttu-id="e95c5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e95c5-115">Application</span></span>|<span data-ttu-id="e95c5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e95c5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e95c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e95c5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}/Release
```

## <a name="request-headers"></a><span data-ttu-id="e95c5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e95c5-118">Request headers</span></span>

|<span data-ttu-id="e95c5-119">名称</span><span class="sxs-lookup"><span data-stu-id="e95c5-119">Name</span></span>|<span data-ttu-id="e95c5-120">说明</span><span class="sxs-lookup"><span data-stu-id="e95c5-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e95c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e95c5-121">Authorization</span></span>|<span data-ttu-id="e95c5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e95c5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e95c5-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e95c5-124">Request body</span></span>

<span data-ttu-id="e95c5-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e95c5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e95c5-126">响应</span><span class="sxs-lookup"><span data-stu-id="e95c5-126">Response</span></span>

<span data-ttu-id="e95c5-127">如果成功，此操作返回 `202 Accepted` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e95c5-127">If successful, this action returns a `202 Accepted` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e95c5-128">示例</span><span class="sxs-lookup"><span data-stu-id="e95c5-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e95c5-129">请求</span><span class="sxs-lookup"><span data-stu-id="e95c5-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "noncustodialdatasource_release"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8e402dd7f3c94a3abc086e5d07db1c6d/release
```

### <a name="response"></a><span data-ttu-id="e95c5-130">响应</span><span class="sxs-lookup"><span data-stu-id="e95c5-130">Response</span></span>

<span data-ttu-id="e95c5-131">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e95c5-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
```
