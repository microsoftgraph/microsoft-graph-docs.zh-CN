---
title: reports： getGroupArchivedPrintJobs
description: 获取特定组的已存档打印作业的列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 2f4a5861e55377548244971edb4c4e02056b55e9
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517244"
---
# <a name="reportroot-getgrouparchivedprintjobs"></a><span data-ttu-id="3c0de-103">reportRoot： getGroupArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="3c0de-103">reportRoot: getGroupArchivedPrintJobs</span></span>
<span data-ttu-id="3c0de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c0de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="3c0de-105">获取特定组的已存档打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="3c0de-105">Get a list of archived print jobs for a particular group.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c0de-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3c0de-106">Permissions</span></span>
<span data-ttu-id="3c0de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c0de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="3c0de-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="3c0de-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="3c0de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c0de-110">Permission type</span></span> | <span data-ttu-id="3c0de-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c0de-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="3c0de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c0de-112">Delegated (work or school account)</span></span>| <span data-ttu-id="3c0de-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c0de-113">Reports.Read.All</span></span> |
|<span data-ttu-id="3c0de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c0de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c0de-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c0de-115">Not Supported.</span></span>|
|<span data-ttu-id="3c0de-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c0de-116">Application</span></span>|<span data-ttu-id="3c0de-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c0de-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c0de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c0de-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getGroupArchivedPrintJobs
```

## <a name="function-parameters"></a><span data-ttu-id="3c0de-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="3c0de-119">Function parameters</span></span>

| <span data-ttu-id="3c0de-120">参数</span><span class="sxs-lookup"><span data-stu-id="3c0de-120">Parameter</span></span>     | <span data-ttu-id="3c0de-121">类型</span><span class="sxs-lookup"><span data-stu-id="3c0de-121">Type</span></span>                 | <span data-ttu-id="3c0de-122">是否必需？</span><span class="sxs-lookup"><span data-stu-id="3c0de-122">Required?</span></span> | <span data-ttu-id="3c0de-123">Description</span><span class="sxs-lookup"><span data-stu-id="3c0de-123">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `groupId`     | `Edm.String`         | <span data-ttu-id="3c0de-124">是</span><span class="sxs-lookup"><span data-stu-id="3c0de-124">Yes</span></span>       | <span data-ttu-id="3c0de-125">要返回其数据的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="3c0de-125">The ID of the group to return data for.</span></span>                              |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="3c0de-126">否</span><span class="sxs-lookup"><span data-stu-id="3c0de-126">No</span></span>        | <span data-ttu-id="3c0de-127">开始日期 (包含) 数据时间段的包含日期。</span><span class="sxs-lookup"><span data-stu-id="3c0de-127">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="3c0de-128">否</span><span class="sxs-lookup"><span data-stu-id="3c0de-128">No</span></span>        | <span data-ttu-id="3c0de-129">结束日期 (包含) 数据的时间段的包含日期。</span><span class="sxs-lookup"><span data-stu-id="3c0de-129">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="request-headers"></a><span data-ttu-id="3c0de-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c0de-130">Request headers</span></span>
|<span data-ttu-id="3c0de-131">名称</span><span class="sxs-lookup"><span data-stu-id="3c0de-131">Name</span></span>|<span data-ttu-id="3c0de-132">说明</span><span class="sxs-lookup"><span data-stu-id="3c0de-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3c0de-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c0de-133">Authorization</span></span>|<span data-ttu-id="3c0de-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c0de-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c0de-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c0de-136">Request body</span></span>
<span data-ttu-id="3c0de-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c0de-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c0de-138">响应</span><span class="sxs-lookup"><span data-stu-id="3c0de-138">Response</span></span>

<span data-ttu-id="3c0de-139">如果成功，此函数在响应正文中返回响应 `200 OK` 代码和 [archivedPrintJob](../resources/archivedprintjob.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="3c0de-139">If successful, this function returns a `200 OK` response code and a [archivedPrintJob](../resources/archivedprintjob.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c0de-140">示例</span><span class="sxs-lookup"><span data-stu-id="3c0de-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c0de-141">请求</span><span class="sxs-lookup"><span data-stu-id="3c0de-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reports_getgrouparchivedprintjobs"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/getGroupArchivedPrintJobs(groupId='{id}',startDateTime=<timestamp>,endDateTime=<timestamp>)
```

### <a name="response"></a><span data-ttu-id="3c0de-142">响应</span><span class="sxs-lookup"><span data-stu-id="3c0de-142">Response</span></span>
<span data-ttu-id="3c0de-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3c0de-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

