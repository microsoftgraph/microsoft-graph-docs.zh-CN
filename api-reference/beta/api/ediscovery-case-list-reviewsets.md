---
title: 列出 reviewSets
description: 从 case 对象获取 reviewSet 资源。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1ef80d6801cad9405d4089c548ef8ad93e0bd794
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776646"
---
# <a name="list-reviewsets"></a><span data-ttu-id="a54cb-103">列出 reviewSets</span><span class="sxs-lookup"><span data-stu-id="a54cb-103">List reviewSets</span></span>

<span data-ttu-id="a54cb-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a54cb-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a54cb-105">从 case[对象获取 reviewSets](../resources/ediscovery-reviewset.md)[列表。](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="a54cb-105">Get the list of [reviewSets](../resources/ediscovery-reviewset.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a54cb-106">权限</span><span class="sxs-lookup"><span data-stu-id="a54cb-106">Permissions</span></span>

<span data-ttu-id="a54cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a54cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a54cb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a54cb-109">Permission type</span></span>|<span data-ttu-id="a54cb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a54cb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a54cb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a54cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a54cb-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a54cb-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a54cb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a54cb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a54cb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a54cb-114">Not supported.</span></span>|
|<span data-ttu-id="a54cb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a54cb-115">Application</span></span>|<span data-ttu-id="a54cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a54cb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a54cb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a54cb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/reviewSets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a54cb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a54cb-118">Optional query parameters</span></span>

<span data-ttu-id="a54cb-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a54cb-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a54cb-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a54cb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a54cb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a54cb-121">Request headers</span></span>

|<span data-ttu-id="a54cb-122">名称</span><span class="sxs-lookup"><span data-stu-id="a54cb-122">Name</span></span>|<span data-ttu-id="a54cb-123">说明</span><span class="sxs-lookup"><span data-stu-id="a54cb-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a54cb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a54cb-124">Authorization</span></span>|<span data-ttu-id="a54cb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a54cb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a54cb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a54cb-127">Request body</span></span>

<span data-ttu-id="a54cb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a54cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a54cb-129">响应</span><span class="sxs-lookup"><span data-stu-id="a54cb-129">Response</span></span>

<span data-ttu-id="a54cb-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a54cb-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a54cb-131">示例</span><span class="sxs-lookup"><span data-stu-id="a54cb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a54cb-132">请求</span><span class="sxs-lookup"><span data-stu-id="a54cb-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a54cb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a54cb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_reviewset"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/reviewSets
```
# <a name="c"></a>[<span data-ttu-id="a54cb-134">C#</span><span class="sxs-lookup"><span data-stu-id="a54cb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-reviewset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a54cb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a54cb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-reviewset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a54cb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a54cb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-reviewset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a54cb-137">Java</span><span class="sxs-lookup"><span data-stu-id="a54cb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-reviewset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a54cb-138">响应</span><span class="sxs-lookup"><span data-stu-id="a54cb-138">Response</span></span>

<span data-ttu-id="a54cb-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a54cb-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
