---
title: 列出 printServices
description: 检索 printService 对象的列表，这些对象代表可供租户使用的服务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b72a2e2a59cfc718832a9082428878c0258d3321
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967056"
---
# <a name="list-printservices"></a><span data-ttu-id="c5c31-103">列出 printServices</span><span class="sxs-lookup"><span data-stu-id="c5c31-103">List printServices</span></span>

<span data-ttu-id="c5c31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5c31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5c31-105">检索 [printService](../resources/printservice.md) 对象的列表，这些对象代表可供租户使用的 **服务** 。</span><span class="sxs-lookup"><span data-stu-id="c5c31-105">Retrieve a list of [printService](../resources/printservice.md) objects that represent the **services** available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5c31-106">权限</span><span class="sxs-lookup"><span data-stu-id="c5c31-106">Permissions</span></span>
<span data-ttu-id="c5c31-107">不需要任何权限即可调用此 API，但若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="c5c31-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c5c31-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5c31-108">Permission type</span></span> | <span data-ttu-id="c5c31-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5c31-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c5c31-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5c31-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c5c31-111">无。</span><span class="sxs-lookup"><span data-stu-id="c5c31-111">None.</span></span>|
|<span data-ttu-id="c5c31-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5c31-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5c31-113">无。</span><span class="sxs-lookup"><span data-stu-id="c5c31-113">None.</span></span>|
|<span data-ttu-id="c5c31-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5c31-114">Application</span></span>|<span data-ttu-id="c5c31-115">无。</span><span class="sxs-lookup"><span data-stu-id="c5c31-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5c31-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5c31-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5c31-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5c31-117">Optional query parameters</span></span>
<span data-ttu-id="c5c31-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5c31-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c5c31-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c5c31-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5c31-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5c31-120">Request headers</span></span>
| <span data-ttu-id="c5c31-121">名称</span><span class="sxs-lookup"><span data-stu-id="c5c31-121">Name</span></span>      |<span data-ttu-id="c5c31-122">说明</span><span class="sxs-lookup"><span data-stu-id="c5c31-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5c31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5c31-123">Authorization</span></span> | <span data-ttu-id="c5c31-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5c31-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5c31-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5c31-126">Request body</span></span>
<span data-ttu-id="c5c31-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5c31-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c5c31-128">响应</span><span class="sxs-lookup"><span data-stu-id="c5c31-128">Response</span></span>
<span data-ttu-id="c5c31-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [printService](../resources/printservice.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c5c31-129">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5c31-130">示例</span><span class="sxs-lookup"><span data-stu-id="c5c31-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5c31-131">请求</span><span class="sxs-lookup"><span data-stu-id="c5c31-131">Request</span></span>
<span data-ttu-id="c5c31-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c5c31-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5c31-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5c31-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services
```
# <a name="c"></a>[<span data-ttu-id="c5c31-134">C#</span><span class="sxs-lookup"><span data-stu-id="c5c31-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5c31-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5c31-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5c31-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5c31-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5c31-137">Java</span><span class="sxs-lookup"><span data-stu-id="c5c31-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c5c31-138">响应</span><span class="sxs-lookup"><span data-stu-id="c5c31-138">Response</span></span>
<span data-ttu-id="c5c31-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c5c31-139">The following is an example of the response.</span></span>
><span data-ttu-id="c5c31-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c5c31-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/services",
  "value": [
    {
      "id": "f4cfee8b-4117-4773-a2f0-3807beb282b9",
      "endpoints": [
        {
          "id": "mpsdiscovery",
          "displayName": "Microsoft Universal Print Discovery Service",
          "uri": "https://discovery.print.microsoft.com"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


