---
title: reports： getPrinterArchivedPrintJobs
description: 获取已排入特定打印机队列的已存档打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: daf0acf2ab9bc285d05aae9f3b875ffc6f329b03
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472408"
---
# <a name="reports-getprinterarchivedprintjobs"></a><span data-ttu-id="9c1a1-103">reports： getPrinterArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="9c1a1-103">reports: getPrinterArchivedPrintJobs</span></span>

<span data-ttu-id="9c1a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c1a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c1a1-105">获取已排入特定打印机队列的已存档打印作业 [的列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-105">Get a list of archived print jobs that were queued for particular [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c1a1-106">权限</span><span class="sxs-lookup"><span data-stu-id="9c1a1-106">Permissions</span></span>
<span data-ttu-id="9c1a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9c1a1-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="9c1a1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c1a1-110">Permission type</span></span> | <span data-ttu-id="9c1a1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c1a1-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9c1a1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c1a1-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9c1a1-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c1a1-113">Reports.Read.All</span></span> |
|<span data-ttu-id="9c1a1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c1a1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c1a1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-115">Not Supported.</span></span>|
|<span data-ttu-id="9c1a1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c1a1-116">Application</span></span>|<span data-ttu-id="9c1a1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c1a1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c1a1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getPrinterArchivedPrintJobs(printerId=printerId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="9c1a1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c1a1-119">Request headers</span></span>
| <span data-ttu-id="9c1a1-120">名称</span><span class="sxs-lookup"><span data-stu-id="9c1a1-120">Name</span></span>          | <span data-ttu-id="9c1a1-121">说明</span><span class="sxs-lookup"><span data-stu-id="9c1a1-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9c1a1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c1a1-122">Authorization</span></span> | <span data-ttu-id="9c1a1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="9c1a1-125">函数参数</span><span class="sxs-lookup"><span data-stu-id="9c1a1-125">Function parameters</span></span>

| <span data-ttu-id="9c1a1-126">参数</span><span class="sxs-lookup"><span data-stu-id="9c1a1-126">Parameter</span></span>     | <span data-ttu-id="9c1a1-127">类型</span><span class="sxs-lookup"><span data-stu-id="9c1a1-127">Type</span></span>                 | <span data-ttu-id="9c1a1-128">是否必需？</span><span class="sxs-lookup"><span data-stu-id="9c1a1-128">Required?</span></span> | <span data-ttu-id="9c1a1-129">说明</span><span class="sxs-lookup"><span data-stu-id="9c1a1-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `printerId`   | `Edm.String`         | <span data-ttu-id="9c1a1-130">是</span><span class="sxs-lookup"><span data-stu-id="9c1a1-130">Yes</span></span>       | <span data-ttu-id="9c1a1-131">要返回其数据的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-131">The ID of the printer to return data for.</span></span>                            |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="9c1a1-132">否</span><span class="sxs-lookup"><span data-stu-id="9c1a1-132">No</span></span>        | <span data-ttu-id="9c1a1-133">开始日期 (包含) 数据时间段的包含日期。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="9c1a1-134">否</span><span class="sxs-lookup"><span data-stu-id="9c1a1-134">No</span></span>        | <span data-ttu-id="9c1a1-135">结束日期 (包含) 数据的时间段的包含日期。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="9c1a1-136">响应</span><span class="sxs-lookup"><span data-stu-id="9c1a1-136">Response</span></span>
<span data-ttu-id="9c1a1-137">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1a1-138">示例</span><span class="sxs-lookup"><span data-stu-id="9c1a1-138">Example</span></span>
<span data-ttu-id="9c1a1-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9c1a1-140">请求</span><span class="sxs-lookup"><span data-stu-id="9c1a1-140">Request</span></span>
<span data-ttu-id="9c1a1-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getprinterarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getPrinterArchivedPrintJobs(printerId='{id}',startDateTime={timestamp},endDateTime={timestamp})
```

##### <a name="response"></a><span data-ttu-id="9c1a1-142">响应</span><span class="sxs-lookup"><span data-stu-id="9c1a1-142">Response</span></span>
<span data-ttu-id="9c1a1-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-143">The following is an example of the response.</span></span>
><span data-ttu-id="9c1a1-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9c1a1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

