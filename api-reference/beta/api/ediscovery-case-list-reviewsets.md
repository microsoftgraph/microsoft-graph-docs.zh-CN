---
title: 列出 reviewSets
description: 从 case 对象获取 reviewSet 资源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: eb881a041ac890cb5c2c616cbf57189e26f8e272
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446094"
---
# <a name="list-reviewsets"></a><span data-ttu-id="568ca-103">列出 reviewSets</span><span class="sxs-lookup"><span data-stu-id="568ca-103">List reviewSets</span></span>

<span data-ttu-id="568ca-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="568ca-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="568ca-105">从 case[对象获取 reviewSets](../resources/ediscovery-reviewset.md)[列表。](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="568ca-105">Get the list of [reviewSets](../resources/ediscovery-reviewset.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="568ca-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="568ca-106">Permissions</span></span>

<span data-ttu-id="568ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="568ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="568ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="568ca-109">Permission type</span></span>|<span data-ttu-id="568ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="568ca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="568ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="568ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="568ca-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="568ca-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="568ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="568ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="568ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="568ca-114">Not supported.</span></span>|
|<span data-ttu-id="568ca-115">Application</span><span class="sxs-lookup"><span data-stu-id="568ca-115">Application</span></span>|<span data-ttu-id="568ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="568ca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="568ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="568ca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/reviewSets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="568ca-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="568ca-118">Optional query parameters</span></span>

<span data-ttu-id="568ca-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="568ca-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="568ca-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="568ca-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="568ca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="568ca-121">Request headers</span></span>

|<span data-ttu-id="568ca-122">名称</span><span class="sxs-lookup"><span data-stu-id="568ca-122">Name</span></span>|<span data-ttu-id="568ca-123">说明</span><span class="sxs-lookup"><span data-stu-id="568ca-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="568ca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="568ca-124">Authorization</span></span>|<span data-ttu-id="568ca-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="568ca-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="568ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="568ca-127">Request body</span></span>

<span data-ttu-id="568ca-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="568ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="568ca-129">响应</span><span class="sxs-lookup"><span data-stu-id="568ca-129">Response</span></span>

<span data-ttu-id="568ca-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="568ca-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="568ca-131">示例</span><span class="sxs-lookup"><span data-stu-id="568ca-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="568ca-132">请求</span><span class="sxs-lookup"><span data-stu-id="568ca-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_reviewset"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/reviewSets
```

### <a name="response"></a><span data-ttu-id="568ca-133">响应</span><span class="sxs-lookup"><span data-stu-id="568ca-133">Response</span></span>

<span data-ttu-id="568ca-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="568ca-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.reviewSet)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#cases",
    "@odata.nextLink": "https://graph.microsoft.com/beta/compliance/ediscovery/cases?$skiptoken=<encodedPageToken>",
    "value": [
        {
            "id": "f6a91542-4ce7-4712-b275-c29545dd8507",
            "displayName": "My Reviewset 1",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T11:58:27.1408174Z"
        },
        {
            "id": "0d78ec4a-aa91-41ea-8da8-d68b030c168f",
            "displayName": "My Reviewset 2",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-01-16T12:03:32.2038960Z"
        }
    ]
}
```
