---
title: 报告： getPrinterArchivedPrintJobs
description: 获取排队等候特定打印机的存档打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a6ff5b6d9031c142821728b31cb66f8b0c5d100f
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845462"
---
# <a name="reports-getprinterarchivedprintjobs"></a><span data-ttu-id="6e89a-103">报告： getPrinterArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="6e89a-103">reports: getPrinterArchivedPrintJobs</span></span>

<span data-ttu-id="6e89a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e89a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e89a-105">获取排队等候特定[打印机](../resources/printer.md)的存档打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="6e89a-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e89a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6e89a-106">Permissions</span></span>
<span data-ttu-id="6e89a-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6e89a-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6e89a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e89a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6e89a-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="6e89a-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="6e89a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e89a-110">Permission type</span></span> | <span data-ttu-id="6e89a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e89a-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6e89a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e89a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="6e89a-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="6e89a-113">Users.Read.All</span></span> |
|<span data-ttu-id="6e89a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e89a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e89a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e89a-115">Not Supported.</span></span>|
|<span data-ttu-id="6e89a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e89a-116">Application</span></span>|<span data-ttu-id="6e89a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e89a-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e89a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e89a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getPrinterArchivedPrintJobs
GET /reports/getPrinterArchivedPrintJobs
```
## <a name="request-headers"></a><span data-ttu-id="6e89a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e89a-119">Request headers</span></span>
| <span data-ttu-id="6e89a-120">名称</span><span class="sxs-lookup"><span data-stu-id="6e89a-120">Name</span></span>          | <span data-ttu-id="6e89a-121">说明</span><span class="sxs-lookup"><span data-stu-id="6e89a-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6e89a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e89a-122">Authorization</span></span> | <span data-ttu-id="6e89a-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6e89a-123">Bearer {token}.</span></span> <span data-ttu-id="6e89a-124">Required.</span><span class="sxs-lookup"><span data-stu-id="6e89a-124">Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="6e89a-125">函数参数</span><span class="sxs-lookup"><span data-stu-id="6e89a-125">Function parameters</span></span>

| <span data-ttu-id="6e89a-126">参数</span><span class="sxs-lookup"><span data-stu-id="6e89a-126">Parameter</span></span>     | <span data-ttu-id="6e89a-127">类型</span><span class="sxs-lookup"><span data-stu-id="6e89a-127">Type</span></span>                 | <span data-ttu-id="6e89a-128">是否必需？</span><span class="sxs-lookup"><span data-stu-id="6e89a-128">Required?</span></span> | <span data-ttu-id="6e89a-129">Description</span><span class="sxs-lookup"><span data-stu-id="6e89a-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="6e89a-130">是</span><span class="sxs-lookup"><span data-stu-id="6e89a-130">Yes</span></span>       | <span data-ttu-id="6e89a-131">要为其返回数据的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="6e89a-131">The ID of the printer to return data for.</span></span>                            |
| `periodStart` | `Edm.DateTimeOffset` | <span data-ttu-id="6e89a-132">否</span><span class="sxs-lookup"><span data-stu-id="6e89a-132">No</span></span>        | <span data-ttu-id="6e89a-133">要在其中包含数据的时间段的开始日期（含）。</span><span class="sxs-lookup"><span data-stu-id="6e89a-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `periodEnd`   | `Edm.DateTimeOffset` | <span data-ttu-id="6e89a-134">否</span><span class="sxs-lookup"><span data-stu-id="6e89a-134">No</span></span>        | <span data-ttu-id="6e89a-135">要在其中包含数据的时间段的结束日期（含）。</span><span class="sxs-lookup"><span data-stu-id="6e89a-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="6e89a-136">响应</span><span class="sxs-lookup"><span data-stu-id="6e89a-136">Response</span></span>
<span data-ttu-id="6e89a-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[archivedPrintJob](../resources/archivedprintjob.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6e89a-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e89a-138">示例</span><span class="sxs-lookup"><span data-stu-id="6e89a-138">Example</span></span>
<span data-ttu-id="6e89a-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6e89a-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6e89a-140">请求</span><span class="sxs-lookup"><span data-stu-id="6e89a-140">Request</span></span>
<span data-ttu-id="6e89a-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e89a-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getprinterarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getPrinterArchivedPrintJobs(printerId='{id}',periodStart=<timestamp>,periodEnd=<timestamp>)
```

##### <a name="response"></a><span data-ttu-id="6e89a-142">响应</span><span class="sxs-lookup"><span data-stu-id="6e89a-142">Response</span></span>
<span data-ttu-id="6e89a-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e89a-143">The following is an example of the response.</span></span>
><span data-ttu-id="6e89a-144">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="6e89a-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6e89a-145">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6e89a-145">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.archivedPrintJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 236

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printer": {
        "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6"
      },
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob: getPrinterArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->