---
title: 获取 printUsageByPrinter
description: 检索特定时间段的打印机使用情况摘要。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 21a282d85a8792f88b3392950582be26726c7400
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774438"
---
# <a name="get-printusagebyprinter"></a><span data-ttu-id="4ec6c-103">获取 printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="4ec6c-103">Get printUsageByPrinter</span></span>
<span data-ttu-id="4ec6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ec6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="4ec6c-105">检索特定时间段的 [打印机](../resources/printer.md) 使用情况摘要。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-105">Retrieve a usage summary for a [printer](../resources/printer.md) for a particular time period.</span></span> <span data-ttu-id="4ec6c-106">有关每个终结点的说明，请参阅 [printUsageByPrinter](../resources/printUsageByPrinter.md)。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-106">For descriptions of each of the endpoints, see [printUsageByPrinter](../resources/printUsageByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ec6c-107">权限</span><span class="sxs-lookup"><span data-stu-id="4ec6c-107">Permissions</span></span>
<span data-ttu-id="4ec6c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4ec6c-110">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="4ec6c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ec6c-111">Permission type</span></span> | <span data-ttu-id="4ec6c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ec6c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4ec6c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ec6c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="4ec6c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ec6c-114">Reports.Read.All</span></span> |
|<span data-ttu-id="4ec6c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ec6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ec6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-116">Not Supported.</span></span>|
|<span data-ttu-id="4ec6c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ec6c-117">Application</span></span>|<span data-ttu-id="4ec6c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ec6c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ec6c-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByPrinter/{id}
GET /reports/monthlyPrintUsageByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ec6c-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ec6c-120">Optional query parameters</span></span>
<span data-ttu-id="4ec6c-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4ec6c-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ec6c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ec6c-123">Request headers</span></span>
|<span data-ttu-id="4ec6c-124">名称</span><span class="sxs-lookup"><span data-stu-id="4ec6c-124">Name</span></span>|<span data-ttu-id="4ec6c-125">说明</span><span class="sxs-lookup"><span data-stu-id="4ec6c-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ec6c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ec6c-126">Authorization</span></span>|<span data-ttu-id="4ec6c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ec6c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ec6c-129">Request body</span></span>
<span data-ttu-id="4ec6c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ec6c-131">响应</span><span class="sxs-lookup"><span data-stu-id="4ec6c-131">Response</span></span>

<span data-ttu-id="4ec6c-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [printUsageByPrinter](../resources/printusagebyprinter.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-132">If successful, this method returns a `200 OK` response code and a [printUsageByPrinter](../resources/printusagebyprinter.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4ec6c-133">示例</span><span class="sxs-lookup"><span data-stu-id="4ec6c-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4ec6c-134">请求</span><span class="sxs-lookup"><span data-stu-id="4ec6c-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4ec6c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ec6c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printusagebyprinter"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByPrinter/{id}
```
# <a name="c"></a>[<span data-ttu-id="4ec6c-136">C#</span><span class="sxs-lookup"><span data-stu-id="4ec6c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagebyprinter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ec6c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ec6c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagebyprinter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ec6c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ec6c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagebyprinter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ec6c-139">Java</span><span class="sxs-lookup"><span data-stu-id="4ec6c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagebyprinter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4ec6c-140">响应</span><span class="sxs-lookup"><span data-stu-id="4ec6c-140">Response</span></span>
<span data-ttu-id="4ec6c-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ec6c-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByPrinter"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
    "usageDate": "Date",
    "completedBlackAndWhiteJobCount": 42,
    "completedColorJobCount": 0,
    "incompleteJobCount": 6
}
```

