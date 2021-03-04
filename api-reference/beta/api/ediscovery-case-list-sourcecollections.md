---
title: 列出 sourceCollections
description: 从 case 对象获取 sourceCollections 资源的列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 10f474b98d8ecde7d12b353ae0bedb4bcebed749
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446092"
---
# <a name="list-sourcecollections"></a><span data-ttu-id="cef6b-103">列出 sourceCollections</span><span class="sxs-lookup"><span data-stu-id="cef6b-103">List sourceCollections</span></span>

<span data-ttu-id="cef6b-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="cef6b-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cef6b-105">从 case[对象获取 sourceCollections](../resources/ediscovery-sourcecollection.md)[列表。](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="cef6b-105">Get the list of [sourceCollections](../resources/ediscovery-sourcecollection.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cef6b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="cef6b-106">Permissions</span></span>

<span data-ttu-id="cef6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cef6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cef6b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cef6b-109">Permission type</span></span>|<span data-ttu-id="cef6b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cef6b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cef6b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cef6b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cef6b-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cef6b-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="cef6b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cef6b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cef6b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cef6b-114">Not supported.</span></span>|
|<span data-ttu-id="cef6b-115">Application</span><span class="sxs-lookup"><span data-stu-id="cef6b-115">Application</span></span>|<span data-ttu-id="cef6b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cef6b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cef6b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cef6b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cef6b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cef6b-118">Optional query parameters</span></span>

<span data-ttu-id="cef6b-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cef6b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cef6b-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cef6b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cef6b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cef6b-121">Request headers</span></span>

|<span data-ttu-id="cef6b-122">名称</span><span class="sxs-lookup"><span data-stu-id="cef6b-122">Name</span></span>|<span data-ttu-id="cef6b-123">说明</span><span class="sxs-lookup"><span data-stu-id="cef6b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cef6b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cef6b-124">Authorization</span></span>|<span data-ttu-id="cef6b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cef6b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cef6b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cef6b-127">Request body</span></span>

<span data-ttu-id="cef6b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cef6b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cef6b-129">响应</span><span class="sxs-lookup"><span data-stu-id="cef6b-129">Response</span></span>

<span data-ttu-id="cef6b-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cef6b-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cef6b-131">示例</span><span class="sxs-lookup"><span data-stu-id="cef6b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cef6b-132">请求</span><span class="sxs-lookup"><span data-stu-id="cef6b-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections
```

### <a name="response"></a><span data-ttu-id="cef6b-133">响应</span><span class="sxs-lookup"><span data-stu-id="cef6b-133">Response</span></span>

<span data-ttu-id="cef6b-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cef6b-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.sourceCollection)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/sourceCollections",
    "value": [
        {
            "description": "",
            "lastModifiedDateTime": "2020-12-31T18:54:28.80694Z",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "contentQuery": "subject:'Quarterly Financials'",
            "tenantSources": "none",
            "id": "fe5ef84e9c8c45819c056f6eb261718e",
            "displayName": "Quarterly Financials",
            "createdDateTime": "2020-12-11T22:56:14.2329133Z"
        }
    ]
}
```
