---
title: 列出保管人 siteSources
description: 获取 siteSource 对象及其属性的列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d8d56f8a82ec4a1dee837c239edc5851d20f1d0a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946259"
---
# <a name="list-custodian-sitesources"></a><span data-ttu-id="e770f-103">列出保管人 siteSources</span><span class="sxs-lookup"><span data-stu-id="e770f-103">List custodian siteSources</span></span>

<span data-ttu-id="e770f-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e770f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e770f-105">获取 [siteSource 对象](../resources/ediscovery-sitesource.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="e770f-105">Get a list of [siteSource](../resources/ediscovery-sitesource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="e770f-106">权限</span><span class="sxs-lookup"><span data-stu-id="e770f-106">Permissions</span></span>

<span data-ttu-id="e770f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e770f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e770f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e770f-109">Permission type</span></span>|<span data-ttu-id="e770f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e770f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e770f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e770f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e770f-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e770f-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e770f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e770f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e770f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e770f-114">Not supported.</span></span>|
|<span data-ttu-id="e770f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e770f-115">Application</span></span>|<span data-ttu-id="e770f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e770f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e770f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e770f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e770f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e770f-118">Optional query parameters</span></span>

<span data-ttu-id="e770f-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e770f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e770f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e770f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e770f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e770f-121">Request headers</span></span>

|<span data-ttu-id="e770f-122">名称</span><span class="sxs-lookup"><span data-stu-id="e770f-122">Name</span></span>|<span data-ttu-id="e770f-123">说明</span><span class="sxs-lookup"><span data-stu-id="e770f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e770f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e770f-124">Authorization</span></span>|<span data-ttu-id="e770f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e770f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e770f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e770f-127">Request body</span></span>

<span data-ttu-id="e770f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e770f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e770f-129">响应</span><span class="sxs-lookup"><span data-stu-id="e770f-129">Response</span></span>

<span data-ttu-id="e770f-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e770f-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e770f-131">示例</span><span class="sxs-lookup"><span data-stu-id="e770f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e770f-132">请求</span><span class="sxs-lookup"><span data-stu-id="e770f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e770f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e770f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sitesource_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
```
# <a name="c"></a>[<span data-ttu-id="e770f-134">C#</span><span class="sxs-lookup"><span data-stu-id="e770f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sitesource-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e770f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e770f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sitesource-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e770f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e770f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sitesource-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e770f-137">Java</span><span class="sxs-lookup"><span data-stu-id="e770f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sitesource-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e770f-138">响应</span><span class="sxs-lookup"><span data-stu-id="e770f-138">Response</span></span>

<span data-ttu-id="e770f-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e770f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "38304445-3741-3333-4233-344238454333",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
