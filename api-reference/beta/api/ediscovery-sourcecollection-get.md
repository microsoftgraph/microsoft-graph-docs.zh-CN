---
title: 获取 sourceCollection
description: 读取 sourceCollection 对象的属性和关系。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1569492ccc7451dffbbd18788ffc41008030f4ed
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080356"
---
# <a name="get-sourcecollection"></a><span data-ttu-id="bda31-103">获取 sourceCollection</span><span class="sxs-lookup"><span data-stu-id="bda31-103">Get sourceCollection</span></span>

<span data-ttu-id="bda31-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="bda31-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bda31-105">读取 [sourceCollection](../resources/ediscovery-sourcecollection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bda31-105">Read the properties and relationships of a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bda31-106">权限</span><span class="sxs-lookup"><span data-stu-id="bda31-106">Permissions</span></span>

<span data-ttu-id="bda31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bda31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bda31-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bda31-109">Permission type</span></span>|<span data-ttu-id="bda31-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bda31-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bda31-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bda31-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bda31-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bda31-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="bda31-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bda31-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bda31-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bda31-114">Not supported.</span></span>|
|<span data-ttu-id="bda31-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bda31-115">Application</span></span>|<span data-ttu-id="bda31-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bda31-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bda31-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bda31-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bda31-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bda31-118">Optional query parameters</span></span>

<span data-ttu-id="bda31-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bda31-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bda31-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="bda31-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="bda31-121">用于 `$expand` 展开审阅集操作、保管人源和上次估计统计信息操作。</span><span class="sxs-lookup"><span data-stu-id="bda31-121">Use `$expand` to expand review set operations, custodian sources, and the last estimate statistics operation.</span></span>

```http
https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```

## <a name="request-headers"></a><span data-ttu-id="bda31-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="bda31-122">Request headers</span></span>

|<span data-ttu-id="bda31-123">名称</span><span class="sxs-lookup"><span data-stu-id="bda31-123">Name</span></span>|<span data-ttu-id="bda31-124">说明</span><span class="sxs-lookup"><span data-stu-id="bda31-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bda31-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bda31-125">Authorization</span></span>|<span data-ttu-id="bda31-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bda31-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bda31-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bda31-128">Request body</span></span>

<span data-ttu-id="bda31-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bda31-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bda31-130">响应</span><span class="sxs-lookup"><span data-stu-id="bda31-130">Response</span></span>

<span data-ttu-id="bda31-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bda31-131">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bda31-132">示例</span><span class="sxs-lookup"><span data-stu-id="bda31-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bda31-133">请求</span><span class="sxs-lookup"><span data-stu-id="bda31-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bda31-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bda31-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sourcecollection"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourcecollections/1a9b4145d8f84e39bc45a7f68c5c5119?$expand=addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation
```
# <a name="c"></a>[<span data-ttu-id="bda31-135">C#</span><span class="sxs-lookup"><span data-stu-id="bda31-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sourcecollection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bda31-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bda31-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sourcecollection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bda31-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bda31-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sourcecollection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bda31-138">Java</span><span class="sxs-lookup"><span data-stu-id="bda31-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sourcecollection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bda31-139">响应</span><span class="sxs-lookup"><span data-stu-id="bda31-139">Response</span></span>

> <span data-ttu-id="bda31-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bda31-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('47746044-fd0b-4a30-acfc-5272b691ba5b')/sourceCollections/$entity",
    "description": null,
    "lastModifiedDateTime": "2021-01-12T18:09:03.7378679Z",
    "contentQuery": "subject:'Quarterly Financials'",
    "dataSourceScopes": "allTenantMailboxes",
    "id": "1a9b4145d8f84e39bc45a7f68c5c5119",
    "displayName": "Quarterly Financials search",
    "createdDateTime": "2021-01-12T18:09:03.417009Z",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": "EDisco Admin",
            "userPrincipalname": "admin@contoso.onmicrosoft.com"
        }
    },
    "addToReviewSetOperation": {
        "createdDateTime": "2021-01-13T05:38:49.9186654Z",
        "completedDateTime": "2021-01-13T07:54:45.0007868Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "addToReviewSet",
        "id": "aef586b34d89405d802497658a14194f",
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": null,
                "userPrincipalName": "admin@contoso.com"
            }
        }
    },
    "lastEstimateStatisticsOperation": {
        "createdDateTime": "2021-01-12T21:53:50.7272654Z",
        "completedDateTime": "2021-01-12T21:54:49.5595543Z",
        "percentProgress": 100,
        "status": "succeeded",
        "action": "estimateStatistics",
        "id": "f3db0382af0842eaa98c7dd59e7dace6",
        "indexedItemCount": 39598,
        "indexedItemsSize": 3760920737,
        "unindexedItemCount": 0,
        "unindexedItemsSize": 0,
        "mailboxCount": 1,
        "siteCount": 1,
        "createdBy": {
            "user": {
                "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                "displayName": "EDisco Admin",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    }
}
```
