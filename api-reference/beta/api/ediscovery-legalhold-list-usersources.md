---
title: 列出 legalHold userSources
description: 从 userSources 导航属性获取 userSource 资源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a87ff92ea60c4d7c048dff91f5fb13c92e040d11
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446041"
---
# <a name="list-legalhold-usersources"></a><span data-ttu-id="86d63-103">列出 legalHold userSources</span><span class="sxs-lookup"><span data-stu-id="86d63-103">List legalHold userSources</span></span>

<span data-ttu-id="86d63-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="86d63-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86d63-105">获取与合法保留相关联的 [userSource](../resources/ediscovery-usersource.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="86d63-105">Get the list of [userSource](../resources/ediscovery-usersource.md) objects associated with a legal hold.</span></span>

## <a name="permissions"></a><span data-ttu-id="86d63-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="86d63-106">Permissions</span></span>

<span data-ttu-id="86d63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86d63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86d63-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86d63-109">Permission type</span></span>|<span data-ttu-id="86d63-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86d63-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86d63-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86d63-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86d63-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86d63-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="86d63-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86d63-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86d63-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86d63-114">Not supported.</span></span>|
|<span data-ttu-id="86d63-115">Application</span><span class="sxs-lookup"><span data-stu-id="86d63-115">Application</span></span>|<span data-ttu-id="86d63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86d63-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86d63-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86d63-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86d63-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="86d63-118">Optional query parameters</span></span>

<span data-ttu-id="86d63-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="86d63-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="86d63-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="86d63-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="86d63-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="86d63-121">Request headers</span></span>

|<span data-ttu-id="86d63-122">名称</span><span class="sxs-lookup"><span data-stu-id="86d63-122">Name</span></span>|<span data-ttu-id="86d63-123">说明</span><span class="sxs-lookup"><span data-stu-id="86d63-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86d63-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="86d63-124">Authorization</span></span>|<span data-ttu-id="86d63-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86d63-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86d63-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="86d63-127">Request body</span></span>

<span data-ttu-id="86d63-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86d63-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86d63-129">响应</span><span class="sxs-lookup"><span data-stu-id="86d63-129">Response</span></span>

<span data-ttu-id="86d63-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="86d63-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86d63-131">示例</span><span class="sxs-lookup"><span data-stu-id="86d63-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86d63-132">请求</span><span class="sxs-lookup"><span data-stu-id="86d63-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/userSources
```

### <a name="response"></a><span data-ttu-id="86d63-133">响应</span><span class="sxs-lookup"><span data-stu-id="86d63-133">Response</span></span>

<span data-ttu-id="86d63-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="86d63-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.userSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalholds('277107ff-fee3-41a0-a665-a9d7f6c4824f')/userSources",
    "value": [
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "2f279b24-2142-435d-97c5-0d42220ba453",
            "email": "AdeleV@contoso.com",
            "includedSources": "mailbox",
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
