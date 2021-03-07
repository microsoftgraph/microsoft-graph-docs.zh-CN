---
title: 列出 dailyPrintUsageByPrinter
description: 检索按打印机分组的每日打印使用率摘要列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 093d1180cacfbbc933fca0f3bc7031085ab5f46a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517306"
---
# <a name="list-dailyprintusagebyprinter"></a><span data-ttu-id="1157b-103">列出 dailyPrintUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="1157b-103">List dailyPrintUsageByPrinter</span></span>
<span data-ttu-id="1157b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1157b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="1157b-105">检索按打印机分组的每日打印使用率摘要 [的列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="1157b-105">Retrieve a list of daily print usage summaries, grouped by [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1157b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1157b-106">Permissions</span></span>
<span data-ttu-id="1157b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1157b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1157b-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="1157b-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="1157b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1157b-110">Permission type</span></span> | <span data-ttu-id="1157b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1157b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1157b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1157b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="1157b-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1157b-113">Reports.Read.All</span></span> |
|<span data-ttu-id="1157b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1157b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1157b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1157b-115">Not Supported.</span></span>|
|<span data-ttu-id="1157b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1157b-116">Application</span></span>|<span data-ttu-id="1157b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1157b-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1157b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1157b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByPrinter
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1157b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1157b-119">Optional query parameters</span></span>
<span data-ttu-id="1157b-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1157b-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1157b-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1157b-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1157b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1157b-122">Request headers</span></span>
|<span data-ttu-id="1157b-123">名称</span><span class="sxs-lookup"><span data-stu-id="1157b-123">Name</span></span>|<span data-ttu-id="1157b-124">说明</span><span class="sxs-lookup"><span data-stu-id="1157b-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1157b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1157b-125">Authorization</span></span>|<span data-ttu-id="1157b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1157b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1157b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1157b-128">Request body</span></span>
<span data-ttu-id="1157b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1157b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1157b-130">响应</span><span class="sxs-lookup"><span data-stu-id="1157b-130">Response</span></span>

<span data-ttu-id="1157b-131">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printUsageByPrinter](../resources/printusagebyprinter.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1157b-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageByPrinter](../resources/printusagebyprinter.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1157b-132">示例</span><span class="sxs-lookup"><span data-stu-id="1157b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1157b-133">请求</span><span class="sxs-lookup"><span data-stu-id="1157b-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printusagebyprinter"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByPrinter
```


### <a name="response"></a><span data-ttu-id="1157b-134">响应</span><span class="sxs-lookup"><span data-stu-id="1157b-134">Response</span></span>
<span data-ttu-id="1157b-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1157b-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printUsageByPrinter)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "usageDate": "Date",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

