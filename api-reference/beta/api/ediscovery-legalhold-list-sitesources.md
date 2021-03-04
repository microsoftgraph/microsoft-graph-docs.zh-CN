---
title: 列出 legalHold siteSources
description: 获取与合法保留相关联的 siteSource 对象列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 2e3be09db4a31a4bb8a3edf86194712f3aa4416c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446042"
---
# <a name="list-legalhold-sitesources"></a><span data-ttu-id="d285d-103">列出 legalHold siteSources</span><span class="sxs-lookup"><span data-stu-id="d285d-103">List legalHold siteSources</span></span>

<span data-ttu-id="d285d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="d285d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d285d-105">获取与合法保留相关联的 [siteSource](../resources/ediscovery-sitesource.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="d285d-105">Get the list of [siteSource](../resources/ediscovery-sitesource.md) objecs associated with a legal hold.</span></span>

## <a name="permissions"></a><span data-ttu-id="d285d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d285d-106">Permissions</span></span>

<span data-ttu-id="d285d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions- reference)。</span><span class="sxs-lookup"><span data-stu-id="d285d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions- reference).</span></span>

|<span data-ttu-id="d285d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d285d-109">Permission type</span></span>|<span data-ttu-id="d285d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d285d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d285d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d285d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d285d-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d285d-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="d285d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d285d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d285d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d285d-114">Not supported.</span></span>|
|<span data-ttu-id="d285d-115">Application</span><span class="sxs-lookup"><span data-stu-id="d285d-115">Application</span></span>|<span data-ttu-id="d285d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d285d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d285d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d285d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d285d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d285d-118">Optional query parameters</span></span>

<span data-ttu-id="d285d-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d285d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d285d-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d285d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d285d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d285d-121">Request headers</span></span>

|<span data-ttu-id="d285d-122">名称</span><span class="sxs-lookup"><span data-stu-id="d285d-122">Name</span></span>|<span data-ttu-id="d285d-123">说明</span><span class="sxs-lookup"><span data-stu-id="d285d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d285d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d285d-124">Authorization</span></span>|<span data-ttu-id="d285d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d285d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d285d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d285d-127">Request body</span></span>

<span data-ttu-id="d285d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d285d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d285d-129">响应</span><span class="sxs-lookup"><span data-stu-id="d285d-129">Response</span></span>

<span data-ttu-id="d285d-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d285d-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d285d-131">示例</span><span class="sxs-lookup"><span data-stu-id="d285d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d285d-132">请求</span><span class="sxs-lookup"><span data-stu-id="d285d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/siteSources
```

### <a name="response"></a><span data-ttu-id="d285d-133">响应</span><span class="sxs-lookup"><span data-stu-id="d285d-133">Response</span></span>

<span data-ttu-id="d285d-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d285d-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.siteSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalHolds('277107ff-fee3-41a0-a665-a9d7f6c4824f')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "43aab990-183e-4593-b772-578bb129e89b",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        },
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "e87b37ac-fad4-471b-9dd8-0e16000a3554",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        }
    ]
}
```
