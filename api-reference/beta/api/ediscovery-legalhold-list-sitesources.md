---
title: 列出 legalHold siteSources
description: 获取与法定保留相关联的 siteSource 对象列表。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 313d47528809eea3ba2cc7e27f7e73114195f992
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773058"
---
# <a name="list-legalhold-sitesources"></a><span data-ttu-id="31664-103">列出 legalHold siteSources</span><span class="sxs-lookup"><span data-stu-id="31664-103">List legalHold siteSources</span></span>

<span data-ttu-id="31664-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="31664-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31664-105">获取与法定保留相关联的 [siteSource](../resources/ediscovery-sitesource.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="31664-105">Get the list of [siteSource](../resources/ediscovery-sitesource.md) objecs associated with a legal hold.</span></span>

## <a name="permissions"></a><span data-ttu-id="31664-106">权限</span><span class="sxs-lookup"><span data-stu-id="31664-106">Permissions</span></span>

<span data-ttu-id="31664-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions- reference)。</span><span class="sxs-lookup"><span data-stu-id="31664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions- reference).</span></span>

|<span data-ttu-id="31664-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="31664-109">Permission type</span></span>|<span data-ttu-id="31664-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31664-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31664-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31664-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31664-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31664-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="31664-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31664-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31664-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="31664-114">Not supported.</span></span>|
|<span data-ttu-id="31664-115">Application</span><span class="sxs-lookup"><span data-stu-id="31664-115">Application</span></span>|<span data-ttu-id="31664-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31664-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31664-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31664-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31664-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31664-118">Optional query parameters</span></span>

<span data-ttu-id="31664-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31664-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="31664-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="31664-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="31664-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="31664-121">Request headers</span></span>

|<span data-ttu-id="31664-122">名称</span><span class="sxs-lookup"><span data-stu-id="31664-122">Name</span></span>|<span data-ttu-id="31664-123">说明</span><span class="sxs-lookup"><span data-stu-id="31664-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="31664-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="31664-124">Authorization</span></span>|<span data-ttu-id="31664-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31664-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31664-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31664-127">Request body</span></span>

<span data-ttu-id="31664-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31664-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31664-129">响应</span><span class="sxs-lookup"><span data-stu-id="31664-129">Response</span></span>

<span data-ttu-id="31664-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="31664-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31664-131">示例</span><span class="sxs-lookup"><span data-stu-id="31664-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31664-132">请求</span><span class="sxs-lookup"><span data-stu-id="31664-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="31664-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="31664-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/siteSources
```
# <a name="c"></a>[<span data-ttu-id="31664-134">C#</span><span class="sxs-lookup"><span data-stu-id="31664-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sitesource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31664-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31664-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sitesource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31664-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31664-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sitesource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31664-137">Java</span><span class="sxs-lookup"><span data-stu-id="31664-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sitesource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31664-138">响应</span><span class="sxs-lookup"><span data-stu-id="31664-138">Response</span></span>

<span data-ttu-id="31664-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="31664-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
