---
title: 报告： getUserArchivedPrintJobs
description: 获取特定用户的已存档打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 017488e472143d66b48ca33732c0ea1d6aa07475
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845440"
---
# <a name="reports-getuserarchivedprintjobs"></a><span data-ttu-id="17620-103">报告： getUserArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="17620-103">reports: getUserArchivedPrintJobs</span></span>

<span data-ttu-id="17620-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17620-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17620-105">获取特定用户的已存档打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="17620-105">Get a list of archived print jobs for a particular user.</span></span>

## <a name="permissions"></a><span data-ttu-id="17620-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="17620-106">Permissions</span></span>
<span data-ttu-id="17620-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="17620-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="17620-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17620-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="17620-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="17620-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="17620-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="17620-110">Permission type</span></span> | <span data-ttu-id="17620-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17620-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="17620-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17620-112">Delegated (work or school account)</span></span>| <span data-ttu-id="17620-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="17620-113">Users.Read.All</span></span> |
|<span data-ttu-id="17620-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17620-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17620-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="17620-115">Not Supported.</span></span>|
|<span data-ttu-id="17620-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="17620-116">Application</span></span>|<span data-ttu-id="17620-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="17620-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17620-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17620-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getUserArchivedPrintJobs
GET /reports/getUserArchivedPrintJobs
```
## <a name="request-headers"></a><span data-ttu-id="17620-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="17620-119">Request headers</span></span>
| <span data-ttu-id="17620-120">名称</span><span class="sxs-lookup"><span data-stu-id="17620-120">Name</span></span>          | <span data-ttu-id="17620-121">说明</span><span class="sxs-lookup"><span data-stu-id="17620-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="17620-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="17620-122">Authorization</span></span> | <span data-ttu-id="17620-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="17620-123">Bearer {token}.</span></span> <span data-ttu-id="17620-124">Required.</span><span class="sxs-lookup"><span data-stu-id="17620-124">Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="17620-125">函数参数</span><span class="sxs-lookup"><span data-stu-id="17620-125">Function Parameters</span></span>

| <span data-ttu-id="17620-126">参数</span><span class="sxs-lookup"><span data-stu-id="17620-126">Parameter</span></span>     | <span data-ttu-id="17620-127">类型</span><span class="sxs-lookup"><span data-stu-id="17620-127">Type</span></span>                 | <span data-ttu-id="17620-128">是否必需？</span><span class="sxs-lookup"><span data-stu-id="17620-128">Required?</span></span> | <span data-ttu-id="17620-129">Description</span><span class="sxs-lookup"><span data-stu-id="17620-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `userId`      | `Edm.String`         | <span data-ttu-id="17620-130">是</span><span class="sxs-lookup"><span data-stu-id="17620-130">Yes</span></span>       | <span data-ttu-id="17620-131">要为其返回数据的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="17620-131">The ID of the user to return data for.</span></span>                               |
| `periodStart` | `Edm.DateTimeOffset` | <span data-ttu-id="17620-132">否</span><span class="sxs-lookup"><span data-stu-id="17620-132">No</span></span>        | <span data-ttu-id="17620-133">要在其中包含数据的时间段的开始日期（含）。</span><span class="sxs-lookup"><span data-stu-id="17620-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `periodEnd`   | `Edm.DateTimeOffset` | <span data-ttu-id="17620-134">否</span><span class="sxs-lookup"><span data-stu-id="17620-134">No</span></span>        | <span data-ttu-id="17620-135">要在其中包含数据的时间段的结束日期（含）。</span><span class="sxs-lookup"><span data-stu-id="17620-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="17620-136">响应</span><span class="sxs-lookup"><span data-stu-id="17620-136">Response</span></span>
<span data-ttu-id="17620-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[archivedPrintJob](../resources/archivedprintjob.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="17620-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17620-138">示例</span><span class="sxs-lookup"><span data-stu-id="17620-138">Example</span></span>
<span data-ttu-id="17620-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="17620-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="17620-140">请求</span><span class="sxs-lookup"><span data-stu-id="17620-140">Request</span></span>
<span data-ttu-id="17620-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17620-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getuserarchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getUserArchivedPrintJobs(userId={id},periodStart=<timestamp>,periodEnd=<timestamp>)
```

##### <a name="response"></a><span data-ttu-id="17620-142">响应</span><span class="sxs-lookup"><span data-stu-id="17620-142">Response</span></span>
<span data-ttu-id="17620-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17620-143">The following is an example of the response.</span></span>
><span data-ttu-id="17620-144">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="17620-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="17620-145">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="17620-145">All the properties will be returned from an actual call.</span></span>
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
  "description": "printJob: getUserArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->