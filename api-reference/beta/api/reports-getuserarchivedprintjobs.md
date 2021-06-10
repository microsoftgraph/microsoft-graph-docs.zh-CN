---
title: reports： getUserArchivedPrintJobs
description: 获取特定用户的已存档打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3a1ed3c1e1965d88db9ab7fd9493c9c747f6b6df
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869559"
---
# <a name="reports-getuserarchivedprintjobs"></a><span data-ttu-id="a9f86-103">reports： getUserArchivedPrintJobs</span><span class="sxs-lookup"><span data-stu-id="a9f86-103">reports: getUserArchivedPrintJobs</span></span>

<span data-ttu-id="a9f86-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9f86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9f86-105">获取特定用户的已存档打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="a9f86-105">Get a list of archived print jobs for a particular user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9f86-106">权限</span><span class="sxs-lookup"><span data-stu-id="a9f86-106">Permissions</span></span>
<span data-ttu-id="a9f86-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9f86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a9f86-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="a9f86-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="a9f86-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9f86-110">Permission type</span></span> | <span data-ttu-id="a9f86-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9f86-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a9f86-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9f86-112">Delegated (work or school account)</span></span>| <span data-ttu-id="a9f86-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9f86-113">Reports.Read.All</span></span> |
|<span data-ttu-id="a9f86-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9f86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9f86-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9f86-115">Not Supported.</span></span>|
|<span data-ttu-id="a9f86-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9f86-116">Application</span></span>|<span data-ttu-id="a9f86-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9f86-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9f86-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9f86-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/reports/getUserArchivedPrintJobs(userId=userId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
GET /reports/getUserArchivedPrintJobs(userId=userId-value,startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```
## <a name="request-headers"></a><span data-ttu-id="a9f86-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9f86-119">Request headers</span></span>
| <span data-ttu-id="a9f86-120">名称</span><span class="sxs-lookup"><span data-stu-id="a9f86-120">Name</span></span>          | <span data-ttu-id="a9f86-121">说明</span><span class="sxs-lookup"><span data-stu-id="a9f86-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a9f86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9f86-122">Authorization</span></span> | <span data-ttu-id="a9f86-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9f86-p102">Bearer {token}. Required.</span></span> |

## <a name="function-parameters"></a><span data-ttu-id="a9f86-125">函数参数</span><span class="sxs-lookup"><span data-stu-id="a9f86-125">Function Parameters</span></span>

| <span data-ttu-id="a9f86-126">参数</span><span class="sxs-lookup"><span data-stu-id="a9f86-126">Parameter</span></span>     | <span data-ttu-id="a9f86-127">类型</span><span class="sxs-lookup"><span data-stu-id="a9f86-127">Type</span></span>                 | <span data-ttu-id="a9f86-128">是否必需？</span><span class="sxs-lookup"><span data-stu-id="a9f86-128">Required?</span></span> | <span data-ttu-id="a9f86-129">说明</span><span class="sxs-lookup"><span data-stu-id="a9f86-129">Description</span></span>                                                          |
|---------------|----------------------|-----------|----------------------------------------------------------------------|
| `userId`      | `Edm.String`         | <span data-ttu-id="a9f86-130">是</span><span class="sxs-lookup"><span data-stu-id="a9f86-130">Yes</span></span>       | <span data-ttu-id="a9f86-131">要返回其数据的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="a9f86-131">The ID of the user to return data for.</span></span>                               |
| `startDateTime` | `Edm.DateTimeOffset` | <span data-ttu-id="a9f86-132">否</span><span class="sxs-lookup"><span data-stu-id="a9f86-132">No</span></span>        | <span data-ttu-id="a9f86-133">开始日期包含 (数据) 时间段的包含时间（含这两者）。</span><span class="sxs-lookup"><span data-stu-id="a9f86-133">The start date (inclusive) for the time period to include data from.</span></span> |
| `endDateTime`   | `Edm.DateTimeOffset` | <span data-ttu-id="a9f86-134">否</span><span class="sxs-lookup"><span data-stu-id="a9f86-134">No</span></span>        | <span data-ttu-id="a9f86-135">结束日期包括 (数据) 时间段的包含时间（含这两者）。</span><span class="sxs-lookup"><span data-stu-id="a9f86-135">The end date (inclusive) for the time period to include data from.</span></span>   |

## <a name="response"></a><span data-ttu-id="a9f86-136">响应</span><span class="sxs-lookup"><span data-stu-id="a9f86-136">Response</span></span>
<span data-ttu-id="a9f86-137">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [archivedPrintJob](../resources/archivedprintjob.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a9f86-137">If successful, this method returns a `200 OK` response code and a collection of [archivedPrintJob](../resources/archivedprintjob.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9f86-138">示例</span><span class="sxs-lookup"><span data-stu-id="a9f86-138">Example</span></span>
<span data-ttu-id="a9f86-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="a9f86-139">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a9f86-140">请求</span><span class="sxs-lookup"><span data-stu-id="a9f86-140">Request</span></span>
<span data-ttu-id="a9f86-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a9f86-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9f86-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9f86-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reports-getuserarchivedprintjobs",
  "sampleKeys": ["016b5565-3bbf-4067-b9ff-4d68167eb1a6"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/reports/getUserArchivedPrintJobs(userId='016b5565-3bbf-4067-b9ff-4d68167eb1a6',startDateTime=2021-05-24,endDateTime=2021-05-25)
```
# <a name="c"></a>[<span data-ttu-id="a9f86-143">C#</span><span class="sxs-lookup"><span data-stu-id="a9f86-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reports-getuserarchivedprintjobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9f86-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9f86-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reports-getuserarchivedprintjobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9f86-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9f86-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reports-getuserarchivedprintjobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9f86-146">Java</span><span class="sxs-lookup"><span data-stu-id="a9f86-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reports-getuserarchivedprintjobs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a9f86-147">响应</span><span class="sxs-lookup"><span data-stu-id="a9f86-147">Response</span></span>
<span data-ttu-id="a9f86-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a9f86-148">The following is an example of the response.</span></span>
><span data-ttu-id="a9f86-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a9f86-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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

