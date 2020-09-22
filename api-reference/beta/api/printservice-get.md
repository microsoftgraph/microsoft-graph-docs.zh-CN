---
title: 获取 printService
description: 检索打印服务的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d4def36af2088469b808e9a12f8cde93556029b4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035367"
---
# <a name="get-printservice"></a><span data-ttu-id="b5674-103">获取 printService</span><span class="sxs-lookup"><span data-stu-id="b5674-103">Get printService</span></span>

<span data-ttu-id="b5674-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5674-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5674-105">检索打印服务的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5674-105">Retrieve the properties and relationships of a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5674-106">权限</span><span class="sxs-lookup"><span data-stu-id="b5674-106">Permissions</span></span>
<span data-ttu-id="b5674-107">不需要任何权限即可调用此 API，但若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="b5674-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="b5674-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5674-108">Permission type</span></span> | <span data-ttu-id="b5674-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5674-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b5674-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5674-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b5674-111">无。</span><span class="sxs-lookup"><span data-stu-id="b5674-111">None.</span></span>|
|<span data-ttu-id="b5674-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5674-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5674-113">无。</span><span class="sxs-lookup"><span data-stu-id="b5674-113">None.</span></span>|
|<span data-ttu-id="b5674-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5674-114">Application</span></span>|<span data-ttu-id="b5674-115">无。</span><span class="sxs-lookup"><span data-stu-id="b5674-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5674-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5674-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5674-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b5674-117">Optional query parameters</span></span>
<span data-ttu-id="b5674-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b5674-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b5674-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b5674-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5674-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5674-120">Request headers</span></span>
| <span data-ttu-id="b5674-121">名称</span><span class="sxs-lookup"><span data-stu-id="b5674-121">Name</span></span>      |<span data-ttu-id="b5674-122">说明</span><span class="sxs-lookup"><span data-stu-id="b5674-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5674-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5674-123">Authorization</span></span> | <span data-ttu-id="b5674-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5674-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5674-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5674-126">Request body</span></span>
<span data-ttu-id="b5674-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5674-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b5674-128">响应</span><span class="sxs-lookup"><span data-stu-id="b5674-128">Response</span></span>
<span data-ttu-id="b5674-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printService](../resources/printservice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5674-129">If successful, this method returns a `200 OK` response code and a [printService](../resources/printservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5674-130">示例</span><span class="sxs-lookup"><span data-stu-id="b5674-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5674-131">请求</span><span class="sxs-lookup"><span data-stu-id="b5674-131">Request</span></span>
<span data-ttu-id="b5674-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b5674-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5674-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5674-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printservice"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}
```
# <a name="c"></a>[<span data-ttu-id="b5674-134">C#</span><span class="sxs-lookup"><span data-stu-id="b5674-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5674-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5674-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5674-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5674-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b5674-137">响应</span><span class="sxs-lookup"><span data-stu-id="b5674-137">Response</span></span>
<span data-ttu-id="b5674-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b5674-138">The following is an example of the response.</span></span>
><span data-ttu-id="b5674-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b5674-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 332

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/services/$entity",
  "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
  "endpoints": [
    {
      "id": "mpsdiscovery",
      "displayName": "Microsoft Universal Print Discovery Service",
      "uri": "https://discovery.print.microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


