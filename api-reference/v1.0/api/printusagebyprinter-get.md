---
title: 获取 printUsageByPrinter
description: 检索特定时间段的打印机使用情况摘要。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9ba1d8a3e91298b87813a9f335bb72482a743b82
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517156"
---
# <a name="get-printusagebyprinter"></a><span data-ttu-id="3c2a1-103">获取 printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="3c2a1-103">Get printUsageByPrinter</span></span>
<span data-ttu-id="3c2a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c2a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="3c2a1-105">检索特定时间段的 [打印机](../resources/printer.md) 使用情况摘要。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-105">Retrieve a usage summary for a [printer](../resources/printer.md) for a particular time period.</span></span> <span data-ttu-id="3c2a1-106">有关每个终结点的说明，请参阅[printUsageByPrinter。](../resources/printUsageByPrinter.md)</span><span class="sxs-lookup"><span data-stu-id="3c2a1-106">For descriptions of each of the endpoints, see [printUsageByPrinter](../resources/printUsageByPrinter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c2a1-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3c2a1-107">Permissions</span></span>
<span data-ttu-id="3c2a1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3c2a1-110">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="3c2a1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c2a1-111">Permission type</span></span> | <span data-ttu-id="3c2a1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c2a1-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3c2a1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c2a1-113">Delegated (work or school account)</span></span>| <span data-ttu-id="3c2a1-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c2a1-114">Reports.Read.All</span></span> |
|<span data-ttu-id="3c2a1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c2a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c2a1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-116">Not Supported.</span></span>|
|<span data-ttu-id="3c2a1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c2a1-117">Application</span></span>|<span data-ttu-id="3c2a1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c2a1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c2a1-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByPrinter/{id}
GET /reports/monthlyPrintUsageByPrinter/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c2a1-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3c2a1-120">Optional query parameters</span></span>
<span data-ttu-id="3c2a1-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3c2a1-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c2a1-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c2a1-123">Request headers</span></span>
|<span data-ttu-id="3c2a1-124">名称</span><span class="sxs-lookup"><span data-stu-id="3c2a1-124">Name</span></span>|<span data-ttu-id="3c2a1-125">说明</span><span class="sxs-lookup"><span data-stu-id="3c2a1-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3c2a1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c2a1-126">Authorization</span></span>|<span data-ttu-id="3c2a1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c2a1-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c2a1-129">Request body</span></span>
<span data-ttu-id="3c2a1-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c2a1-131">响应</span><span class="sxs-lookup"><span data-stu-id="3c2a1-131">Response</span></span>

<span data-ttu-id="3c2a1-132">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printUsageByPrinter](../resources/printusagebyprinter.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-132">If successful, this method returns a `200 OK` response code and a [printUsageByPrinter](../resources/printusagebyprinter.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c2a1-133">示例</span><span class="sxs-lookup"><span data-stu-id="3c2a1-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c2a1-134">请求</span><span class="sxs-lookup"><span data-stu-id="3c2a1-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printusagebyprinter"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByPrinter/{id}
```


### <a name="response"></a><span data-ttu-id="3c2a1-135">响应</span><span class="sxs-lookup"><span data-stu-id="3c2a1-135">Response</span></span>
<span data-ttu-id="3c2a1-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3c2a1-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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

