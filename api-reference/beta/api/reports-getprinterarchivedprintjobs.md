---
title: reports： getPrinterArchivedPrintJobs
description: 获取已排队等待特定打印机的存档打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8c779775284a98ae5e68a6b57bb773c7a1753264
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780972"
---
# <a name="reports-getprinterarchivedprintjobs"></a><span data-ttu-id="22d67-103">reports： getPrinterArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="22d67-103">reports: getPrinterArchivedPrintJobs</span></span>

<span data-ttu-id="22d67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d67-105">获取已排队等待特定打印机的存档打印作业 [的列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="22d67-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="22d67-106">权限</span><span class="sxs-lookup"><span data-stu-id="22d67-106">Permissions</span></span>
<span data-ttu-id="22d67-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22d67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="22d67-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="22d67-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="22d67-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="22d67-110">Permission type</span></span> | <span data-ttu-id="22d67-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22d67-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="22d67-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22d67-112">Delegated (work or school account)</span></span>| <span data-ttu-id="22d67-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="22d67-113">Reports.Read.All</span></span> |
|<span data-ttu-id="22d67-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22d67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22d67-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="22d67-115">Not Supported.</span></span>|
|<span data-ttu-id="22d67-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="22d67-116">Application</span></span>|<span data-ttu-id="22d67-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="22d67-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22d67-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22d67-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="22d67-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="22d67-119">Request headers</span></span>
| <span data-ttu-id="22d67-120">名称</span><span class="sxs-lookup"><span data-stu-id="22d67-120">Name</span></span>          | <span data-ttu-id="22d67-121">说明</span><span class="sxs-lookup"><span data-stu-id="22d67-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="22d67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22d67-122">Authorization</span></span> | <span data-ttu-id="22d67-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22d67-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="22d67-125">函数参数</span><span class="sxs-lookup"><span data-stu-id="22d67-125">Function parameters</span></span>

| <span data-ttu-id="22d67-126">参数</span><span class="sxs-lookup"><span data-stu-id="22d67-126">Parameter</span></span>     | <span data-ttu-id="22d67-127">类型</span><span class="sxs-lookup"><span data-stu-id="22d67-127">Type</span></span>                 | <span data-ttu-id="22d67-128">是否必需？</span><span class="sxs-lookup"><span data-stu-id="22d67-128">Required?</span></span> | <span data-ttu-id="22d67-129">说明</span><span class="sxs-lookup"><span data-stu-id="22d67-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="22d67-130">是</span><span class="sxs-lookup"><span data-stu-id="22d67-130">Yes</span></span>       | <span data-ttu-id="22d67-131">要返回其数据的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="22d67-131">The ID of the printer to return data for.</span></span>                            |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="22d67-132">否</span><span class="sxs-lookup"><span data-stu-id="22d67-132">No</span></span>        | <span data-ttu-id="22d67-133">开始日期包含 (数据) 时间段的包含时间（含这两者）。</span><span class="sxs-lookup"><span data-stu-id="22d67-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="22d67-134">否</span><span class="sxs-lookup"><span data-stu-id="22d67-134">No</span></span>        | <span data-ttu-id="22d67-135">结束日期包括 (数据) 时间段的包含时间（含这两者）。</span><span class="sxs-lookup"><span data-stu-id="22d67-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="22d67-136">响应</span><span class="sxs-lookup"><span data-stu-id="22d67-136">Response</span></span>
<span data-ttu-id="22d67-137">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="22d67-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22d67-138">示例</span><span class="sxs-lookup"><span data-stu-id="22d67-138">Example</span></span>
<span data-ttu-id="22d67-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="22d67-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="22d67-140">请求</span><span class="sxs-lookup"><span data-stu-id="22d67-140">Request</span></span>
<span data-ttu-id="22d67-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="22d67-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getprinterarchivedprintjobs",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getPrinterArchivedPrintJobs(printerId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)
```

##### <a name="response"></a><span data-ttu-id="22d67-142">响应</span><span class="sxs-lookup"><span data-stu-id="22d67-142">Response</span></span>
<span data-ttu-id="22d67-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="22d67-143">The following is an example of the response.</span></span>
><span data-ttu-id="22d67-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="22d67-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

