---
title: 列出 addToReviewSetOperation
description: 获取与源集合关联的最后一个 addToReviewSetOperation 对象。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f5ef3f5831e04e125bd67de070c6089cfce90ce0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772665"
---
# <a name="list-addtoreviewsetoperation"></a><span data-ttu-id="37f20-103">列出 addToReviewSetOperation</span><span class="sxs-lookup"><span data-stu-id="37f20-103">List addToReviewSetOperation</span></span>

<span data-ttu-id="37f20-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="37f20-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37f20-105">获取与源集合关联的最后一个 [addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37f20-105">Get the last [addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) object associated with a source collection.</span></span> 

><span data-ttu-id="37f20-106">**注意：** 此方法仅列出最后一个操作;它不会返回所有操作历史记录。</span><span class="sxs-lookup"><span data-stu-id="37f20-106">**Note:** This method only lists the last operation; it does not return a history of all operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="37f20-107">权限</span><span class="sxs-lookup"><span data-stu-id="37f20-107">Permissions</span></span>

<span data-ttu-id="37f20-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37f20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f20-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="37f20-110">Permission type</span></span>|<span data-ttu-id="37f20-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37f20-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37f20-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37f20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37f20-113">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f20-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="37f20-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37f20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37f20-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="37f20-115">Not supported.</span></span>|
|<span data-ttu-id="37f20-116">Application</span><span class="sxs-lookup"><span data-stu-id="37f20-116">Application</span></span>|<span data-ttu-id="37f20-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="37f20-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37f20-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37f20-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/addToReviewSetOperation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37f20-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="37f20-119">Optional query parameters</span></span>

<span data-ttu-id="37f20-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="37f20-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="37f20-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="37f20-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="37f20-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="37f20-122">Request headers</span></span>

|<span data-ttu-id="37f20-123">名称</span><span class="sxs-lookup"><span data-stu-id="37f20-123">Name</span></span>|<span data-ttu-id="37f20-124">说明</span><span class="sxs-lookup"><span data-stu-id="37f20-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37f20-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="37f20-125">Authorization</span></span>|<span data-ttu-id="37f20-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37f20-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37f20-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="37f20-128">Request body</span></span>

<span data-ttu-id="37f20-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="37f20-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37f20-130">响应</span><span class="sxs-lookup"><span data-stu-id="37f20-130">Response</span></span>

<span data-ttu-id="37f20-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37f20-131">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37f20-132">示例</span><span class="sxs-lookup"><span data-stu-id="37f20-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37f20-133">请求</span><span class="sxs-lookup"><span data-stu-id="37f20-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37f20-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="37f20-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_addtoreviewsetoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/addToReviewSetOperation
```
# <a name="c"></a>[<span data-ttu-id="37f20-135">C#</span><span class="sxs-lookup"><span data-stu-id="37f20-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-addtoreviewsetoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37f20-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37f20-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-addtoreviewsetoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37f20-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37f20-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-addtoreviewsetoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37f20-138">Java</span><span class="sxs-lookup"><span data-stu-id="37f20-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-addtoreviewsetoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37f20-139">响应</span><span class="sxs-lookup"><span data-stu-id="37f20-139">Response</span></span>

<span data-ttu-id="37f20-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="37f20-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.addToReviewSetOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.addToReviewSetOperation",
      "id": "9055c657-c657-9055-57c6-559057c65590",
      "createdDateTime": "String (timestamp)",
      "completedDateTime": "String (timestamp)",
      "percentProgress": "Integer",
      "status": "String",
      "action": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo"
      }
    }
  ]
}
```
