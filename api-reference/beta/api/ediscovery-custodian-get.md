---
title: 获取保管人
description: 读取保管人对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 569db93ccd197d5b2cce86e6a69b7fcabbb34aac
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446063"
---
# <a name="get-custodian"></a><span data-ttu-id="c0159-103">获取保管人</span><span class="sxs-lookup"><span data-stu-id="c0159-103">Get custodian</span></span>

<span data-ttu-id="c0159-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c0159-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0159-105">读取保管人对象 [的属性](../resources/ediscovery-custodian.md) 和关系。</span><span class="sxs-lookup"><span data-stu-id="c0159-105">Read the properties and relationships of a [custodian](../resources/ediscovery-custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0159-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c0159-106">Permissions</span></span>

<span data-ttu-id="c0159-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0159-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0159-109">Permission type</span></span>|<span data-ttu-id="c0159-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0159-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0159-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0159-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0159-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0159-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c0159-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0159-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0159-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0159-114">Not supported.</span></span>|
|<span data-ttu-id="c0159-115">Application</span><span class="sxs-lookup"><span data-stu-id="c0159-115">Application</span></span>|<span data-ttu-id="c0159-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0159-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0159-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0159-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caesId}/custodians/{custodianId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0159-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c0159-118">Optional query parameters</span></span>

<span data-ttu-id="c0159-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c0159-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c0159-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c0159-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0159-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0159-121">Request headers</span></span>

|<span data-ttu-id="c0159-122">名称</span><span class="sxs-lookup"><span data-stu-id="c0159-122">Name</span></span>|<span data-ttu-id="c0159-123">说明</span><span class="sxs-lookup"><span data-stu-id="c0159-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c0159-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0159-124">Authorization</span></span>|<span data-ttu-id="c0159-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0159-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0159-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0159-127">Request body</span></span>

<span data-ttu-id="c0159-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0159-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0159-129">响应</span><span class="sxs-lookup"><span data-stu-id="c0159-129">Response</span></span>

<span data-ttu-id="c0159-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0159-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0159-131">示例</span><span class="sxs-lookup"><span data-stu-id="c0159-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0159-132">请求</span><span class="sxs-lookup"><span data-stu-id="c0159-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_custodian"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
```

### <a name="response"></a><span data-ttu-id="c0159-133">响应</span><span class="sxs-lookup"><span data-stu-id="c0159-133">Response</span></span>

<span data-ttu-id="c0159-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c0159-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.custodian"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": true,
    "status": "active",
    "createdDateTime": "2020-10-30T20:59:54.9900703Z",
    "lastModifiedDateTime": "2020-10-30T20:59:55.1400013Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45454331323337443946343043464239",
    "displayName": "Adele Vance"
}
```
