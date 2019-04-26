---
title: 'reportRoot: getSharePointActivityUserDetail'
description: 获取用户执行的 SharePoint 活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7df02b2f9124a77d7113ccd711a3c2f0a50bac7f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332210"
---
# <a name="reportroot-getsharepointactivityuserdetail"></a><span data-ttu-id="4ce46-103">reportRoot: getSharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4ce46-103">reportRoot: getSharePointActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ce46-104">获取用户执行的 SharePoint 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4ce46-104">Get details about SharePoint activity by user.</span></span>

> <span data-ttu-id="4ce46-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。</span><span class="sxs-lookup"><span data-stu-id="4ce46-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint activity](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ce46-106">权限</span><span class="sxs-lookup"><span data-stu-id="4ce46-106">Permissions</span></span>

<span data-ttu-id="4ce46-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ce46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ce46-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ce46-109">Permission type</span></span>                        | <span data-ttu-id="4ce46-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ce46-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="4ce46-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ce46-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ce46-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ce46-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="4ce46-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ce46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ce46-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ce46-114">Not supported.</span></span>                           |
| <span data-ttu-id="4ce46-115">应用</span><span class="sxs-lookup"><span data-stu-id="4ce46-115">Application</span></span>                            | <span data-ttu-id="4ce46-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ce46-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4ce46-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ce46-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointActivityUserDetail(period='{period_value}')
GET /reports/getSharePointActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="4ce46-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="4ce46-118">Function parameters</span></span>

<span data-ttu-id="4ce46-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="4ce46-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="4ce46-120">参数</span><span class="sxs-lookup"><span data-stu-id="4ce46-120">Parameter</span></span> | <span data-ttu-id="4ce46-121">类型</span><span class="sxs-lookup"><span data-stu-id="4ce46-121">Type</span></span>   | <span data-ttu-id="4ce46-122">说明</span><span class="sxs-lookup"><span data-stu-id="4ce46-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="4ce46-123">period</span><span class="sxs-lookup"><span data-stu-id="4ce46-123">period</span></span>    | <span data-ttu-id="4ce46-124">string</span><span class="sxs-lookup"><span data-stu-id="4ce46-124">string</span></span> | <span data-ttu-id="4ce46-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4ce46-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="4ce46-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="4ce46-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="4ce46-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="4ce46-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="4ce46-128">date</span><span class="sxs-lookup"><span data-stu-id="4ce46-128">date</span></span>      | <span data-ttu-id="4ce46-129">Date</span><span class="sxs-lookup"><span data-stu-id="4ce46-129">Date</span></span>   | <span data-ttu-id="4ce46-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="4ce46-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="4ce46-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="4ce46-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="4ce46-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="4ce46-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="4ce46-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="4ce46-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="4ce46-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4ce46-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="4ce46-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="4ce46-135">The default output type is text/csv.</span></span> <span data-ttu-id="4ce46-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="4ce46-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ce46-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ce46-137">Request headers</span></span>

| <span data-ttu-id="4ce46-138">名称</span><span class="sxs-lookup"><span data-stu-id="4ce46-138">Name</span></span>          | <span data-ttu-id="4ce46-139">说明</span><span class="sxs-lookup"><span data-stu-id="4ce46-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="4ce46-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ce46-140">Authorization</span></span> | <span data-ttu-id="4ce46-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ce46-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4ce46-143">响应</span><span class="sxs-lookup"><span data-stu-id="4ce46-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="4ce46-144">CSV</span><span class="sxs-lookup"><span data-stu-id="4ce46-144">CSV</span></span>

<span data-ttu-id="4ce46-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="4ce46-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="4ce46-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="4ce46-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="4ce46-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="4ce46-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="4ce46-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="4ce46-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="4ce46-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="4ce46-149">Report Refresh Date</span></span>
- <span data-ttu-id="4ce46-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="4ce46-150">User Principal Name</span></span>
- <span data-ttu-id="4ce46-151">已删除</span><span class="sxs-lookup"><span data-stu-id="4ce46-151">Is Deleted</span></span>
- <span data-ttu-id="4ce46-152">删除日期</span><span class="sxs-lookup"><span data-stu-id="4ce46-152">Deleted Date</span></span>
- <span data-ttu-id="4ce46-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="4ce46-153">Last Activity Date</span></span>
- <span data-ttu-id="4ce46-154">已查看或编辑文件数</span><span class="sxs-lookup"><span data-stu-id="4ce46-154">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="4ce46-155">已同步文件数</span><span class="sxs-lookup"><span data-stu-id="4ce46-155">Synced File Count</span></span>
- <span data-ttu-id="4ce46-156">已内部共享文件数</span><span class="sxs-lookup"><span data-stu-id="4ce46-156">Shared Internally File Count</span></span>
- <span data-ttu-id="4ce46-157">已外部共享文件数</span><span class="sxs-lookup"><span data-stu-id="4ce46-157">Shared Externally File Count</span></span>
- <span data-ttu-id="4ce46-158">访问过的页面数</span><span class="sxs-lookup"><span data-stu-id="4ce46-158">Visited Page Count</span></span>
- <span data-ttu-id="4ce46-159">分配的产品</span><span class="sxs-lookup"><span data-stu-id="4ce46-159">Assigned Products</span></span>
- <span data-ttu-id="4ce46-160">报表周期</span><span class="sxs-lookup"><span data-stu-id="4ce46-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="4ce46-161">JSON</span><span class="sxs-lookup"><span data-stu-id="4ce46-161">JSON</span></span>

<span data-ttu-id="4ce46-162">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="4ce46-162">If successful, this method returns a `200 OK` response code and a **[sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="4ce46-163">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="4ce46-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="4ce46-164">示例</span><span class="sxs-lookup"><span data-stu-id="4ce46-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="4ce46-165">CSV</span><span class="sxs-lookup"><span data-stu-id="4ce46-165">CSV</span></span>

<span data-ttu-id="4ce46-166">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="4ce46-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="4ce46-167">请求</span><span class="sxs-lookup"><span data-stu-id="4ce46-167">Request</span></span>

<span data-ttu-id="4ce46-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ce46-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="4ce46-169">响应</span><span class="sxs-lookup"><span data-stu-id="4ce46-169">Response</span></span>

<span data-ttu-id="4ce46-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4ce46-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="4ce46-171">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="4ce46-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Visited Page Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="4ce46-172">JSON</span><span class="sxs-lookup"><span data-stu-id="4ce46-172">JSON</span></span>

<span data-ttu-id="4ce46-173">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="4ce46-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="4ce46-174">请求</span><span class="sxs-lookup"><span data-stu-id="4ce46-174">Request</span></span>

<span data-ttu-id="4ce46-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ce46-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="4ce46-176">响应</span><span class="sxs-lookup"><span data-stu-id="4ce46-176">Response</span></span>

<span data-ttu-id="4ce46-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4ce46-177">The following is an example of the response.</span></span>

> <span data-ttu-id="4ce46-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4ce46-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 473

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 4, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "visitedPageCount": 1, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
