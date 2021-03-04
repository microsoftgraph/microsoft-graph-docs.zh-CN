---
title: 列出保管人
description: 获取保管人对象及其属性的列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: c1f9bd5ffd6c046cd3403fb4ece6e7c23cc2a66a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446100"
---
# <a name="list-custodians"></a><span data-ttu-id="5dd70-103">列出保管人</span><span class="sxs-lookup"><span data-stu-id="5dd70-103">List custodians</span></span>

<span data-ttu-id="5dd70-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="5dd70-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dd70-105">获取保管人 [对象及其](../resources/ediscovery-custodian.md) 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="5dd70-105">Get a list of the [custodian](../resources/ediscovery-custodian.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dd70-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="5dd70-106">Permissions</span></span>

<span data-ttu-id="5dd70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5dd70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dd70-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dd70-109">Permission type</span></span>|<span data-ttu-id="5dd70-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5dd70-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dd70-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dd70-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5dd70-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dd70-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="5dd70-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dd70-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dd70-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dd70-114">Not supported.</span></span>|
|<span data-ttu-id="5dd70-115">Application</span><span class="sxs-lookup"><span data-stu-id="5dd70-115">Application</span></span>|<span data-ttu-id="5dd70-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dd70-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dd70-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dd70-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5dd70-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5dd70-118">Optional query parameters</span></span>

<span data-ttu-id="5dd70-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5dd70-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5dd70-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5dd70-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5dd70-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dd70-121">Request headers</span></span>

|<span data-ttu-id="5dd70-122">名称</span><span class="sxs-lookup"><span data-stu-id="5dd70-122">Name</span></span>|<span data-ttu-id="5dd70-123">说明</span><span class="sxs-lookup"><span data-stu-id="5dd70-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5dd70-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dd70-124">Authorization</span></span>|<span data-ttu-id="5dd70-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5dd70-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dd70-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dd70-127">Request body</span></span>

<span data-ttu-id="5dd70-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5dd70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dd70-129">响应</span><span class="sxs-lookup"><span data-stu-id="5dd70-129">Response</span></span>

<span data-ttu-id="5dd70-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5dd70-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5dd70-131">示例</span><span class="sxs-lookup"><span data-stu-id="5dd70-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5dd70-132">请求</span><span class="sxs-lookup"><span data-stu-id="5dd70-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_custodian"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
```

### <a name="response"></a><span data-ttu-id="5dd70-133">响应</span><span class="sxs-lookup"><span data-stu-id="5dd70-133">Response</span></span>

<span data-ttu-id="5dd70-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5dd70-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.custodian)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians",
    "value": [
        {
            "email": "meganb@contoso.com",
            "applyHoldToSources": false,
            "status": "released",
            "createdDateTime": "2020-10-27T15:55:43.4971108Z",
            "lastModifiedDateTime": "2020-10-30T05:34:00.947558Z",
            "releasedDateTime": "2020-10-27T15:55:58.2338864Z",
            "acknowledgedDateTime": null,
            "id": "fd03ce02ecde42a58d24fcbc9ebbea3e",
            "displayName": "Megan Bowen"
        },
        {
            "email": "AdeleV@contoso.com",
            "applyHoldToSources": true,
            "status": "active",
            "createdDateTime": "2020-08-21T13:20:02.0117254Z",
            "lastModifiedDateTime": "2020-10-27T15:14:14.1244649Z",
            "releasedDateTime": null,
            "acknowledgedDateTime": null,
            "id": "2192ca408ea2410eba3bec8ae873be6b",
            "displayName": "Adele Vance"
        }
    ]
}
```
