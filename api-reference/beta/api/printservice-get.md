---
title: 获取 printService
description: 检索打印服务的属性和关系。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2735e019d4e861bb0a2fc066f3c4796011745d9b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968204"
---
# <a name="get-printservice"></a><span data-ttu-id="3fa56-103">获取 printService</span><span class="sxs-lookup"><span data-stu-id="3fa56-103">Get printService</span></span>

<span data-ttu-id="3fa56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fa56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fa56-105">检索打印服务的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3fa56-105">Retrieve the properties and relationships of a print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fa56-106">权限</span><span class="sxs-lookup"><span data-stu-id="3fa56-106">Permissions</span></span>
<span data-ttu-id="3fa56-107">不需要任何权限即可调用此 API，但若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="3fa56-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="3fa56-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3fa56-108">Permission type</span></span> | <span data-ttu-id="3fa56-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3fa56-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3fa56-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3fa56-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3fa56-111">无。</span><span class="sxs-lookup"><span data-stu-id="3fa56-111">None.</span></span>|
|<span data-ttu-id="3fa56-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3fa56-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fa56-113">无。</span><span class="sxs-lookup"><span data-stu-id="3fa56-113">None.</span></span>|
|<span data-ttu-id="3fa56-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3fa56-114">Application</span></span>|<span data-ttu-id="3fa56-115">无。</span><span class="sxs-lookup"><span data-stu-id="3fa56-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fa56-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3fa56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fa56-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3fa56-117">Optional query parameters</span></span>
<span data-ttu-id="3fa56-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3fa56-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3fa56-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3fa56-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fa56-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3fa56-120">Request headers</span></span>
| <span data-ttu-id="3fa56-121">名称</span><span class="sxs-lookup"><span data-stu-id="3fa56-121">Name</span></span>      |<span data-ttu-id="3fa56-122">说明</span><span class="sxs-lookup"><span data-stu-id="3fa56-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3fa56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fa56-123">Authorization</span></span> | <span data-ttu-id="3fa56-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3fa56-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3fa56-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3fa56-126">Request body</span></span>
<span data-ttu-id="3fa56-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3fa56-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3fa56-128">响应</span><span class="sxs-lookup"><span data-stu-id="3fa56-128">Response</span></span>
<span data-ttu-id="3fa56-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printService](../resources/printservice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3fa56-129">If successful, this method returns a `200 OK` response code and a [printService](../resources/printservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3fa56-130">示例</span><span class="sxs-lookup"><span data-stu-id="3fa56-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3fa56-131">请求</span><span class="sxs-lookup"><span data-stu-id="3fa56-131">Request</span></span>
<span data-ttu-id="3fa56-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3fa56-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3fa56-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3fa56-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printservice"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services/{id}
```
# <a name="c"></a>[<span data-ttu-id="3fa56-134">C#</span><span class="sxs-lookup"><span data-stu-id="3fa56-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3fa56-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3fa56-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3fa56-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3fa56-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3fa56-137">Java</span><span class="sxs-lookup"><span data-stu-id="3fa56-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3fa56-138">响应</span><span class="sxs-lookup"><span data-stu-id="3fa56-138">Response</span></span>
<span data-ttu-id="3fa56-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3fa56-139">The following is an example of the response.</span></span>
><span data-ttu-id="3fa56-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3fa56-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


