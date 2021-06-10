---
title: 获取 printUsageByUser
description: 检索特定时间段的用户使用情况摘要。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ab81ab84a1ff70a0de7fbfb6fce33f83d0260466
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869840"
---
# <a name="get-printusagebyuser"></a><span data-ttu-id="994bf-103">获取 printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="994bf-103">Get printUsageByUser</span></span>

<span data-ttu-id="994bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="994bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="994bf-105">检索特定时间段的用户使用情况摘要。</span><span class="sxs-lookup"><span data-stu-id="994bf-105">Retrieve a user's usage summary for a particular time period.</span></span> 

<span data-ttu-id="994bf-106">有关 [每个终结点的说明，请参阅 printUsageByUser](../resources/printUsageByUser.md) 文档。</span><span class="sxs-lookup"><span data-stu-id="994bf-106">See the [printUsageByUser](../resources/printUsageByUser.md) documentation for descriptions of each of the endpoints.</span></span>

## <a name="permissions"></a><span data-ttu-id="994bf-107">权限</span><span class="sxs-lookup"><span data-stu-id="994bf-107">Permissions</span></span>
<span data-ttu-id="994bf-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="994bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="994bf-110">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="994bf-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="994bf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="994bf-111">Permission type</span></span> | <span data-ttu-id="994bf-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="994bf-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="994bf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="994bf-113">Delegated (work or school account)</span></span>| <span data-ttu-id="994bf-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="994bf-114">Reports.Read.All</span></span> |
|<span data-ttu-id="994bf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="994bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="994bf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="994bf-116">Not Supported.</span></span>|
|<span data-ttu-id="994bf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="994bf-117">Application</span></span>|<span data-ttu-id="994bf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="994bf-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="994bf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="994bf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageByUser/{id}
GET /reports/monthlyPrintUsageByUser/{id}
GET /print/reports/dailyPrintUsageByUser/{id}
GET /print/reports/monthlyPrintUsageByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="994bf-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="994bf-120">Optional query parameters</span></span>
<span data-ttu-id="994bf-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="994bf-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="994bf-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="994bf-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="994bf-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="994bf-123">Request headers</span></span>
| <span data-ttu-id="994bf-124">名称</span><span class="sxs-lookup"><span data-stu-id="994bf-124">Name</span></span>      |<span data-ttu-id="994bf-125">说明</span><span class="sxs-lookup"><span data-stu-id="994bf-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="994bf-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="994bf-126">Authorization</span></span> | <span data-ttu-id="994bf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="994bf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="994bf-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="994bf-129">Request body</span></span>
<span data-ttu-id="994bf-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="994bf-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="994bf-131">响应</span><span class="sxs-lookup"><span data-stu-id="994bf-131">Response</span></span>
<span data-ttu-id="994bf-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printUsageByUser](../resources/printUsageByUser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="994bf-132">If successful, this method returns a `200 OK` response code and a [printUsageByUser](../resources/printUsageByUser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="994bf-133">示例</span><span class="sxs-lookup"><span data-stu-id="994bf-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="994bf-134">请求</span><span class="sxs-lookup"><span data-stu-id="994bf-134">Request</span></span>
<span data-ttu-id="994bf-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="994bf-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="994bf-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="994bf-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printUsageByUser",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageByUser/016b5565-3bbf-4067-b9ff-4d68167eb1a6
```
# <a name="c"></a>[<span data-ttu-id="994bf-137">C#</span><span class="sxs-lookup"><span data-stu-id="994bf-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagebyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="994bf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="994bf-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagebyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="994bf-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="994bf-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagebyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="994bf-140">Java</span><span class="sxs-lookup"><span data-stu-id="994bf-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagebyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="994bf-141">响应</span><span class="sxs-lookup"><span data-stu-id="994bf-141">Response</span></span>
<span data-ttu-id="994bf-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="994bf-142">The following is an example of the response.</span></span>
><span data-ttu-id="994bf-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="994bf-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "userPrincipalName": "username@contoso.com",
  "usageDate": "2020-02-04T00:00:00.0000000Z",
  "completedBlackAndWhiteJobCount": 42,
  "completedColorJobCount": 0,
  "incompleteJobCount": 6
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printUsageByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

