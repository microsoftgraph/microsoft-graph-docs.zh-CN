---
title: 列出 noncustodialDataSources
description: 获取 noncustodialDataSource 对象及其属性的列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 89f083456e2ee67296dcd76699f7b977f030d3ed
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240929"
---
# <a name="list-noncustodialdatasources"></a><span data-ttu-id="e9f86-103">列出 noncustodialDataSources</span><span class="sxs-lookup"><span data-stu-id="e9f86-103">List noncustodialDataSources</span></span>

<span data-ttu-id="e9f86-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e9f86-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9f86-105">获取 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="e9f86-105">Get a list of the [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9f86-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9f86-106">Permissions</span></span>

<span data-ttu-id="e9f86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9f86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9f86-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9f86-109">Permission type</span></span>|<span data-ttu-id="e9f86-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9f86-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9f86-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9f86-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e9f86-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9f86-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e9f86-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9f86-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9f86-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9f86-114">Not supported.</span></span>|
|<span data-ttu-id="e9f86-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9f86-115">Application</span></span>|<span data-ttu-id="e9f86-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9f86-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9f86-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9f86-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/noncustodialDataSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e9f86-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e9f86-118">Optional query parameters</span></span>

<span data-ttu-id="e9f86-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e9f86-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e9f86-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e9f86-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e9f86-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9f86-121">Request headers</span></span>

|<span data-ttu-id="e9f86-122">名称</span><span class="sxs-lookup"><span data-stu-id="e9f86-122">Name</span></span>|<span data-ttu-id="e9f86-123">说明</span><span class="sxs-lookup"><span data-stu-id="e9f86-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e9f86-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9f86-124">Authorization</span></span>|<span data-ttu-id="e9f86-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9f86-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9f86-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9f86-127">Request body</span></span>

<span data-ttu-id="e9f86-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e9f86-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9f86-129">响应</span><span class="sxs-lookup"><span data-stu-id="e9f86-129">Response</span></span>

<span data-ttu-id="e9f86-130">如果成功，此方法在响应正文中返回 响应代码和非 `200 OK` [custodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e9f86-130">If successful, this method returns a `200 OK` response code and a collection of [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9f86-131">示例</span><span class="sxs-lookup"><span data-stu-id="e9f86-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9f86-132">请求</span><span class="sxs-lookup"><span data-stu-id="e9f86-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e9f86-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9f86-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_noncustodialdatasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources
```
# <a name="c"></a>[<span data-ttu-id="e9f86-134">C#</span><span class="sxs-lookup"><span data-stu-id="e9f86-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-noncustodialdatasource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9f86-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9f86-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-noncustodialdatasource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9f86-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9f86-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-noncustodialdatasource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e9f86-137">Java</span><span class="sxs-lookup"><span data-stu-id="e9f86-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-noncustodialdatasource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9f86-138">响应</span><span class="sxs-lookup"><span data-stu-id="e9f86-138">Response</span></span>

<span data-ttu-id="e9f86-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e9f86-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.noncustodialDataSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources",
    "value": [
        {
            "status": "Active",
            "lastModifiedDateTime": "2021-02-17T19:41:28.9144454Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "8e402dd7f3c94a3abc086e5d07db1c6d",
            "displayName": null,
            "createdDateTime": "2021-02-17T19:41:22.9690997Z",
            "applyHoldToSource": true
        },
        {
            "status": "Active",
            "lastModifiedDateTime": "2021-02-17T19:41:28.8714643Z",
            "releasedDateTime": "0001-01-01T00:00:00Z",
            "id": "8b69818bf6af4f8a9dede428401c71e7",
            "displayName": null,
            "createdDateTime": "2021-02-17T19:41:22.958104Z",
            "applyHoldToSource": true
        }
    ]
}
```
