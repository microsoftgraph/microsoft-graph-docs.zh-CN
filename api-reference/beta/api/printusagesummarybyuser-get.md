---
title: 获取 printUsageSummaryByUser
description: 检索特定时间段的用户使用情况摘要。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 20cb026334e88dc6113db579be07a9de01dfaaa7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441391"
---
# <a name="get-printusagesummarybyuser"></a><span data-ttu-id="31719-103">获取 printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="31719-103">Get printUsageSummaryByUser</span></span>

<span data-ttu-id="31719-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31719-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31719-105">检索特定时间段的用户使用情况摘要。</span><span class="sxs-lookup"><span data-stu-id="31719-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="31719-106">有关 [每个终结点的说明，请参阅 printUsageSummaryByUser](../resources/printUsageSummaryByUser.md) 文档。</span><span class="sxs-lookup"><span data-stu-id="31719-106">See the [printUsageSummaryByUser](../resources/printUsageSummaryByUser.md) documentation for descriptions of each of the endpoints.</span></span>

## <a name="permissions"></a><span data-ttu-id="31719-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="31719-107">Permissions</span></span>
<span data-ttu-id="31719-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31719-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="31719-110">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="31719-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="31719-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="31719-111">Permission type</span></span> | <span data-ttu-id="31719-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31719-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="31719-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31719-113">Delegated (work or school account)</span></span>| <span data-ttu-id="31719-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="31719-114">Reports.Read.All</span></span> |
|<span data-ttu-id="31719-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31719-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31719-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31719-116">Not Supported.</span></span>|
|<span data-ttu-id="31719-117">Application</span><span class="sxs-lookup"><span data-stu-id="31719-117">Application</span></span>|<span data-ttu-id="31719-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="31719-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31719-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31719-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /reports/dailyPrintUsageSummariesByUser/{id}
GET /reports/monthlyPrintUsageSummariesByUser/{id}
GET /print/reports/dailyPrintUsageSummariesByUser/{id}
GET /print/reports/monthlyPrintUsageSummariesByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31719-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="31719-120">Optional query parameters</span></span>
<span data-ttu-id="31719-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="31719-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="31719-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="31719-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="31719-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="31719-123">Request headers</span></span>
| <span data-ttu-id="31719-124">名称</span><span class="sxs-lookup"><span data-stu-id="31719-124">Name</span></span>      |<span data-ttu-id="31719-125">说明</span><span class="sxs-lookup"><span data-stu-id="31719-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="31719-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="31719-126">Authorization</span></span> | <span data-ttu-id="31719-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31719-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31719-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="31719-129">Request body</span></span>
<span data-ttu-id="31719-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="31719-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="31719-131">响应</span><span class="sxs-lookup"><span data-stu-id="31719-131">Response</span></span>
<span data-ttu-id="31719-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31719-132">If successful, this method returns a `200 OK` response code and a [printUsageSummaryByUser](../resources/printusagesummarybyuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="31719-133">示例</span><span class="sxs-lookup"><span data-stu-id="31719-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="31719-134">请求</span><span class="sxs-lookup"><span data-stu-id="31719-134">Request</span></span>
<span data-ttu-id="31719-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="31719-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31719-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="31719-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printUsageSummaryByUser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/dailyPrintUsageSummariesByUser/{id}
```
# <a name="c"></a>[<span data-ttu-id="31719-137">C#</span><span class="sxs-lookup"><span data-stu-id="31719-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagesummarybyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31719-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31719-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagesummarybyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31719-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31719-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagesummarybyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31719-140">Java</span><span class="sxs-lookup"><span data-stu-id="31719-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagesummarybyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="31719-141">响应</span><span class="sxs-lookup"><span data-stu-id="31719-141">Response</span></span>
<span data-ttu-id="31719-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="31719-142">The following is an example of the response.</span></span>
><span data-ttu-id="31719-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="31719-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
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
  "description": "Get printUsageSummaryByUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

