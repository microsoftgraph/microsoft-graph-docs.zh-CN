---
title: 获取 siteSource
description: 读取 siteSource 对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a0060509c38e68ab33820032261229439aa48351
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446014"
---
# <a name="get-sitesource"></a><span data-ttu-id="4cb92-103">获取 siteSource</span><span class="sxs-lookup"><span data-stu-id="4cb92-103">Get siteSource</span></span>

<span data-ttu-id="4cb92-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4cb92-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cb92-105">读取 [siteSource](../resources/ediscovery-sitesource.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4cb92-105">Read the properties and relationships of a [siteSource](../resources/ediscovery-sitesource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cb92-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4cb92-106">Permissions</span></span>

<span data-ttu-id="4cb92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4cb92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cb92-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4cb92-109">Permission type</span></span>|<span data-ttu-id="4cb92-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4cb92-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cb92-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4cb92-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4cb92-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cb92-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="4cb92-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4cb92-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cb92-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cb92-114">Not supported.</span></span>|
|<span data-ttu-id="4cb92-115">Application</span><span class="sxs-lookup"><span data-stu-id="4cb92-115">Application</span></span>|<span data-ttu-id="4cb92-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cb92-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cb92-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4cb92-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources/{siteSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4cb92-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4cb92-118">Optional query parameters</span></span>

<span data-ttu-id="4cb92-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4cb92-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4cb92-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4cb92-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cb92-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4cb92-121">Request headers</span></span>

|<span data-ttu-id="4cb92-122">名称</span><span class="sxs-lookup"><span data-stu-id="4cb92-122">Name</span></span>|<span data-ttu-id="4cb92-123">说明</span><span class="sxs-lookup"><span data-stu-id="4cb92-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4cb92-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cb92-124">Authorization</span></span>|<span data-ttu-id="4cb92-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4cb92-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cb92-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4cb92-127">Request body</span></span>

<span data-ttu-id="4cb92-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4cb92-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cb92-129">响应</span><span class="sxs-lookup"><span data-stu-id="4cb92-129">Response</span></span>

<span data-ttu-id="4cb92-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4cb92-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4cb92-131">示例</span><span class="sxs-lookup"><span data-stu-id="4cb92-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4cb92-132">请求</span><span class="sxs-lookup"><span data-stu-id="4cb92-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources/38304445-3741-3333-4233-344238454333
```

### <a name="response"></a><span data-ttu-id="4cb92-133">响应</span><span class="sxs-lookup"><span data-stu-id="4cb92-133">Response</span></span>

<span data-ttu-id="4cb92-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4cb92-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.siteSource"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "displayName": "Human resources site",
    "createdDateTime": "2020-10-27T15:14:11.0048392Z",
    "id": "38304445-3741-3333-4233-344238454333",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null
        }
    }
}
```
