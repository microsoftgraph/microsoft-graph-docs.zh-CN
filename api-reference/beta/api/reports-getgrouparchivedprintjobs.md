---
title: reports： getGroupArchivedPrintJobs
description: 获取特定组的已存档打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 98e208816a2415f176407d1d76194046c0284250
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470807"
---
# <a name="reports-getgrouparchivedprintjobs"></a><span data-ttu-id="72f82-103">reports： getGroupArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="72f82-103">reports: getGroupArchivedPrintJobs</span></span>

<span data-ttu-id="72f82-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72f82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72f82-105">获取特定组的已存档打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="72f82-105">Get a list of archived print jobs for a particular group.</span></span>

## <a name="permissions"></a><span data-ttu-id="72f82-106">权限</span><span class="sxs-lookup"><span data-stu-id="72f82-106">Permissions</span></span>
<span data-ttu-id="72f82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72f82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="72f82-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="72f82-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="72f82-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="72f82-110">Permission type</span></span> | <span data-ttu-id="72f82-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="72f82-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="72f82-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72f82-112">Delegated (work or school account)</span></span>| <span data-ttu-id="72f82-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="72f82-113">Reports.Read.All</span></span> |
|<span data-ttu-id="72f82-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72f82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72f82-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="72f82-115">Not Supported.</span></span>|
|<span data-ttu-id="72f82-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="72f82-116">Application</span></span>|<span data-ttu-id="72f82-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="72f82-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72f82-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72f82-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getGroupArchivedPrintJobs(groupId=groupId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getGroupArchivedPrintJobs(groupId=groupId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="72f82-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="72f82-119">Request headers</span></span>
| <span data-ttu-id="72f82-120">名称</span><span class="sxs-lookup"><span data-stu-id="72f82-120">Name</span></span>          | <span data-ttu-id="72f82-121">说明</span><span class="sxs-lookup"><span data-stu-id="72f82-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="72f82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72f82-122">Authorization</span></span> | <span data-ttu-id="72f82-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72f82-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="72f82-125">函数参数</span><span class="sxs-lookup"><span data-stu-id="72f82-125">Function parameters</span></span>

| <span data-ttu-id="72f82-126">参数</span><span class="sxs-lookup"><span data-stu-id="72f82-126">Parameter</span></span>     | <span data-ttu-id="72f82-127">类型</span><span class="sxs-lookup"><span data-stu-id="72f82-127">Type</span></span>                 | <span data-ttu-id="72f82-128">是否必需？</span><span class="sxs-lookup"><span data-stu-id="72f82-128">Required?</span></span> | <span data-ttu-id="72f82-129">说明</span><span class="sxs-lookup"><span data-stu-id="72f82-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `groupId`     | `Edm.String`         | <span data-ttu-id="72f82-130">是</span><span class="sxs-lookup"><span data-stu-id="72f82-130">Yes</span></span>       | <span data-ttu-id="72f82-131">要返回其数据的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="72f82-131">The ID of the group to return data for.</span></span>                              |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="72f82-132">否</span><span class="sxs-lookup"><span data-stu-id="72f82-132">No</span></span>        | <span data-ttu-id="72f82-133">开始日期 (包含) 数据时间段的包含日期。</span><span class="sxs-lookup"><span data-stu-id="72f82-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="72f82-134">否</span><span class="sxs-lookup"><span data-stu-id="72f82-134">No</span></span>        | <span data-ttu-id="72f82-135">结束日期 (包含) 数据的时间段的包含日期。</span><span class="sxs-lookup"><span data-stu-id="72f82-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="72f82-136">响应</span><span class="sxs-lookup"><span data-stu-id="72f82-136">Response</span></span>
<span data-ttu-id="72f82-137">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="72f82-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72f82-138">示例</span><span class="sxs-lookup"><span data-stu-id="72f82-138">Example</span></span>
<span data-ttu-id="72f82-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="72f82-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="72f82-140">请求</span><span class="sxs-lookup"><span data-stu-id="72f82-140">Request</span></span>
<span data-ttu-id="72f82-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="72f82-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "reports-getgrouparchivedprintjobs"
}-->
```http
GET https://graph.microsoft.com/beta/print/reports/getGroupArchivedPrintJobs(groupId='{id}',startDateTime={timestamp},endDateTime={timestamp})
```

##### <a name="response"></a><span data-ttu-id="72f82-142">响应</span><span class="sxs-lookup"><span data-stu-id="72f82-142">Response</span></span>
<span data-ttu-id="72f82-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="72f82-143">The following is an example of the response.</span></span>
><span data-ttu-id="72f82-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="72f82-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "printJob: getGroupArchivedPrintJobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

