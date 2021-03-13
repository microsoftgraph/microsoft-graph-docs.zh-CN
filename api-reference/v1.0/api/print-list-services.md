---
title: 列出 printServices
description: 检索 printService 对象的列表，这些对象代表可供租户使用的服务。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 72bc0f46df6eccd5462a776f0d38aa70175ab6f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777213"
---
# <a name="list-printservices"></a><span data-ttu-id="8454c-103">列出 printServices</span><span class="sxs-lookup"><span data-stu-id="8454c-103">List printServices</span></span>
<span data-ttu-id="8454c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8454c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="8454c-105">检索 **printService 对象** 的列表，这些对象代表可供租户使用的服务。</span><span class="sxs-lookup"><span data-stu-id="8454c-105">Retrieve a list of **printService** objects that represent the services available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8454c-106">权限</span><span class="sxs-lookup"><span data-stu-id="8454c-106">Permissions</span></span>
<span data-ttu-id="8454c-107">调用 **此** API 需要委派 [的通用打印权限](/graph/permissions-reference#universal-print-permissions) 之一。</span><span class="sxs-lookup"><span data-stu-id="8454c-107">One of the **delegated** Universal Print [permissions](/graph/permissions-reference#universal-print-permissions) is required to call this API.</span></span>

## <a name="http-request"></a><span data-ttu-id="8454c-108">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8454c-108">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8454c-109">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8454c-109">Optional query parameters</span></span>
<span data-ttu-id="8454c-110">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8454c-110">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8454c-111">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="8454c-111">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8454c-112">请求标头</span><span class="sxs-lookup"><span data-stu-id="8454c-112">Request headers</span></span>
|<span data-ttu-id="8454c-113">名称</span><span class="sxs-lookup"><span data-stu-id="8454c-113">Name</span></span>|<span data-ttu-id="8454c-114">说明</span><span class="sxs-lookup"><span data-stu-id="8454c-114">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8454c-115">Authorization</span><span class="sxs-lookup"><span data-stu-id="8454c-115">Authorization</span></span>|<span data-ttu-id="8454c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8454c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8454c-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="8454c-118">Request body</span></span>
<span data-ttu-id="8454c-119">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8454c-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8454c-120">响应</span><span class="sxs-lookup"><span data-stu-id="8454c-120">Response</span></span>

<span data-ttu-id="8454c-121">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printService](../resources/printservice.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8454c-121">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8454c-122">示例</span><span class="sxs-lookup"><span data-stu-id="8454c-122">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8454c-123">请求</span><span class="sxs-lookup"><span data-stu-id="8454c-123">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8454c-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="8454c-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printservice"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/services
```
# <a name="c"></a>[<span data-ttu-id="8454c-125">C#</span><span class="sxs-lookup"><span data-stu-id="8454c-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8454c-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8454c-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8454c-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8454c-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8454c-128">Java</span><span class="sxs-lookup"><span data-stu-id="8454c-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8454c-129">响应</span><span class="sxs-lookup"><span data-stu-id="8454c-129">Response</span></span>
<span data-ttu-id="8454c-130">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8454c-130">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printService)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/services",
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

