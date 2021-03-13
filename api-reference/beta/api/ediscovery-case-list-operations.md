---
title: 列出操作
description: 从 case 对象获取 list caseOperations。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: ee95efa24aa1f7a3c0254e3da2e22cc43e3568c4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776681"
---
# <a name="list-operations"></a><span data-ttu-id="73019-103">列出操作</span><span class="sxs-lookup"><span data-stu-id="73019-103">List operations</span></span>

<span data-ttu-id="73019-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="73019-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73019-105">从 case[对象获取 caseOperations](../resources/ediscovery-caseoperation.md)[列表。](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="73019-105">Get the list of [caseOperations](../resources/ediscovery-caseoperation.md) from a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73019-106">权限</span><span class="sxs-lookup"><span data-stu-id="73019-106">Permissions</span></span>

<span data-ttu-id="73019-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73019-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73019-109">Permission type</span></span>|<span data-ttu-id="73019-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73019-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73019-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73019-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73019-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73019-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="73019-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73019-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73019-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73019-114">Not supported.</span></span>|
|<span data-ttu-id="73019-115">Application</span><span class="sxs-lookup"><span data-stu-id="73019-115">Application</span></span>|<span data-ttu-id="73019-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="73019-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73019-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73019-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/operations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73019-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73019-118">Optional query parameters</span></span>

<span data-ttu-id="73019-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73019-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="73019-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="73019-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="73019-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="73019-121">Request headers</span></span>

|<span data-ttu-id="73019-122">名称</span><span class="sxs-lookup"><span data-stu-id="73019-122">Name</span></span>|<span data-ttu-id="73019-123">说明</span><span class="sxs-lookup"><span data-stu-id="73019-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="73019-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="73019-124">Authorization</span></span>|<span data-ttu-id="73019-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73019-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73019-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="73019-127">Request body</span></span>
<span data-ttu-id="73019-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73019-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73019-129">响应</span><span class="sxs-lookup"><span data-stu-id="73019-129">Response</span></span>

<span data-ttu-id="73019-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="73019-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.caseOperation](../resources/ediscovery-caseoperation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73019-131">示例</span><span class="sxs-lookup"><span data-stu-id="73019-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73019-132">请求</span><span class="sxs-lookup"><span data-stu-id="73019-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="73019-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="73019-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_caseoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/operations
```
# <a name="c"></a>[<span data-ttu-id="73019-134">C#</span><span class="sxs-lookup"><span data-stu-id="73019-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-caseoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73019-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73019-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-caseoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73019-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73019-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-caseoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73019-137">Java</span><span class="sxs-lookup"><span data-stu-id="73019-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-caseoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73019-138">响应</span><span class="sxs-lookup"><span data-stu-id="73019-138">Response</span></span>

<span data-ttu-id="73019-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="73019-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.caseOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
      "id": "41362b70-2b70-4136-702b-3641702b3641",
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
