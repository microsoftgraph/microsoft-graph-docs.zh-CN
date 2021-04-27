---
title: 列出 printServices
description: 检索 printService 对象的列表，这些对象代表可供租户使用的服务。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 3461665b6d027fdba0ecd88e97af422b4f3865ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051093"
---
# <a name="list-printservices"></a><span data-ttu-id="9c9ee-103">列出 printServices</span><span class="sxs-lookup"><span data-stu-id="9c9ee-103">List printServices</span></span>

<span data-ttu-id="9c9ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c9ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c9ee-105">检索 [printService 对象](../resources/printservice.md) 的列表，这些对象 **代表** 可供租户使用的服务。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-105">Retrieve a list of [printService](../resources/printservice.md) objects that represent the **services** available to your tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c9ee-106">权限</span><span class="sxs-lookup"><span data-stu-id="9c9ee-106">Permissions</span></span>
<span data-ttu-id="9c9ee-107">调用此 API 不需要任何权限，但若要使用通用打印服务，用户或应用的租户必须拥有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-107">No permissions are needed to call this API, but to use the Universal Print service, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="9c9ee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c9ee-108">Permission type</span></span> | <span data-ttu-id="9c9ee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c9ee-109">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9c9ee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c9ee-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9c9ee-111">无。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-111">None.</span></span>|
|<span data-ttu-id="9c9ee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c9ee-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c9ee-113">无。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-113">None.</span></span>|
|<span data-ttu-id="9c9ee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c9ee-114">Application</span></span>|<span data-ttu-id="9c9ee-115">无。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-115">None.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c9ee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c9ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/services
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c9ee-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9c9ee-117">Optional query parameters</span></span>
<span data-ttu-id="9c9ee-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9c9ee-119">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c9ee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c9ee-120">Request headers</span></span>
| <span data-ttu-id="9c9ee-121">名称</span><span class="sxs-lookup"><span data-stu-id="9c9ee-121">Name</span></span>      |<span data-ttu-id="9c9ee-122">说明</span><span class="sxs-lookup"><span data-stu-id="9c9ee-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9c9ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c9ee-123">Authorization</span></span> | <span data-ttu-id="9c9ee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c9ee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c9ee-126">Request body</span></span>
<span data-ttu-id="9c9ee-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9c9ee-128">响应</span><span class="sxs-lookup"><span data-stu-id="9c9ee-128">Response</span></span>
<span data-ttu-id="9c9ee-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printService](../resources/printservice.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-129">If successful, this method returns a `200 OK` response code and a collection of [printService](../resources/printservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c9ee-130">示例</span><span class="sxs-lookup"><span data-stu-id="9c9ee-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c9ee-131">请求</span><span class="sxs-lookup"><span data-stu-id="9c9ee-131">Request</span></span>
<span data-ttu-id="9c9ee-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c9ee-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c9ee-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/services
```
# <a name="c"></a>[<span data-ttu-id="9c9ee-134">C#</span><span class="sxs-lookup"><span data-stu-id="9c9ee-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c9ee-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c9ee-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c9ee-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c9ee-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c9ee-137">Java</span><span class="sxs-lookup"><span data-stu-id="9c9ee-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9c9ee-138">响应</span><span class="sxs-lookup"><span data-stu-id="9c9ee-138">Response</span></span>
<span data-ttu-id="9c9ee-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-139">The following is an example of the response.</span></span>
><span data-ttu-id="9c9ee-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9c9ee-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


