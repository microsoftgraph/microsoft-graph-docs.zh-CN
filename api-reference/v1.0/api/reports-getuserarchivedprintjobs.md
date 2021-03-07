---
title: reports： getUserArchivedPrintJobs
description: 获取特定用户的已存档打印作业列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f55a90939d5328075532695ff2af3416e27c5085
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517237"
---
# <a name="reportroot-getuserarchivedprintjobs"></a><span data-ttu-id="a4d8e-103">reportRoot： getUserArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="a4d8e-103">reportRoot: getUserArchivedPrintJobs</span></span>
<span data-ttu-id="a4d8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4d8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a4d8e-105">获取特定用户的已存档打印作业列表。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-105">Get a list of archived print jobs for a particular user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4d8e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a4d8e-106">Permissions</span></span>
<span data-ttu-id="a4d8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a4d8e-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="a4d8e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4d8e-110">Permission type</span></span> | <span data-ttu-id="a4d8e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4d8e-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a4d8e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4d8e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="a4d8e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4d8e-113">Reports.Read.All</span></span> |
|<span data-ttu-id="a4d8e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4d8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4d8e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-115">Not Supported.</span></span>|
|<span data-ttu-id="a4d8e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4d8e-116">Application</span></span>|<span data-ttu-id="a4d8e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4d8e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4d8e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getUserArchivedPrintJobs
```

## <a name="function-parameters"></a><span data-ttu-id="a4d8e-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="a4d8e-119">Function Parameters</span></span>

| <span data-ttu-id="a4d8e-120">参数</span><span class="sxs-lookup"><span data-stu-id="a4d8e-120">Parameter</span></span>     | <span data-ttu-id="a4d8e-121">类型</span><span class="sxs-lookup"><span data-stu-id="a4d8e-121">Type</span></span>                 | <span data-ttu-id="a4d8e-122">是否必需？</span><span class="sxs-lookup"><span data-stu-id="a4d8e-122">Required?</span></span> | <span data-ttu-id="a4d8e-123">Description</span><span class="sxs-lookup"><span data-stu-id="a4d8e-123">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `userId`      | `Edm.String`         | <span data-ttu-id="a4d8e-124">是</span><span class="sxs-lookup"><span data-stu-id="a4d8e-124">Yes</span></span>       | <span data-ttu-id="a4d8e-125">要返回其数据的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-125">The ID of the user to return data for.</span></span>                               |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="a4d8e-126">否</span><span class="sxs-lookup"><span data-stu-id="a4d8e-126">No</span></span>        | <span data-ttu-id="a4d8e-127">开始日期 (包含) 数据时间段的包含日期。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-127">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="a4d8e-128">否</span><span class="sxs-lookup"><span data-stu-id="a4d8e-128">No</span></span>        | <span data-ttu-id="a4d8e-129">结束日期 (包含) 数据的时间段的包含日期。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-129">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="request-headers"></a><span data-ttu-id="a4d8e-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4d8e-130">Request headers</span></span>
|<span data-ttu-id="a4d8e-131">名称</span><span class="sxs-lookup"><span data-stu-id="a4d8e-131">Name</span></span>|<span data-ttu-id="a4d8e-132">说明</span><span class="sxs-lookup"><span data-stu-id="a4d8e-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4d8e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4d8e-133">Authorization</span></span>|<span data-ttu-id="a4d8e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4d8e-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4d8e-136">Request body</span></span>
<span data-ttu-id="a4d8e-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4d8e-138">响应</span><span class="sxs-lookup"><span data-stu-id="a4d8e-138">Response</span></span>

<span data-ttu-id="a4d8e-139">如果成功，此函数在响应正文中返回响应代码和 `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-139">If successful, this function returns a `200 OK` response code and a [archivedPrintJob](../resources/archivedprintjob.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4d8e-140">示例</span><span class="sxs-lookup"><span data-stu-id="a4d8e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4d8e-141">请求</span><span class="sxs-lookup"><span data-stu-id="a4d8e-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reportroot_getuserarchivedprintjobs"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/getUserArchivedPrintJobs(userId='{id}',startDateTime=<timestamp>,endDateTime=<timestamp>)
```

### <a name="response"></a><span data-ttu-id="a4d8e-142">响应</span><span class="sxs-lookup"><span data-stu-id="a4d8e-142">Response</span></span>
<span data-ttu-id="a4d8e-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a4d8e-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.archivedPrintJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "printerId": "fe6ff85a-f0d3-4c4f-aec6-b9d5154356a1",
      "createdBy": {},
      "processingState": "completed"
    }
  ]
}
```

