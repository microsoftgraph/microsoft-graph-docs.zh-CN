---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: 获取用户执行的 OneDrive 活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 1ca242a4c0b653f347ac46d2c6b01435bf1d1d36
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981275"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="d5117-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d5117-103">reportRoot: getOneDriveActivityUserDetail</span></span>

<span data-ttu-id="d5117-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5117-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5117-105">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d5117-105">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="d5117-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="d5117-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5117-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d5117-107">Permissions</span></span>

<span data-ttu-id="d5117-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5117-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5117-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5117-110">Permission type</span></span>                        | <span data-ttu-id="d5117-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5117-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d5117-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5117-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5117-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5117-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d5117-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5117-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5117-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5117-115">Not supported.</span></span>                           |
| <span data-ttu-id="d5117-116">应用</span><span class="sxs-lookup"><span data-stu-id="d5117-116">Application</span></span>                            | <span data-ttu-id="d5117-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5117-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="d5117-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="d5117-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d5117-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="d5117-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d5117-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5117-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d5117-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="d5117-121">Function parameters</span></span>

<span data-ttu-id="d5117-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d5117-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d5117-123">参数</span><span class="sxs-lookup"><span data-stu-id="d5117-123">Parameter</span></span> | <span data-ttu-id="d5117-124">类型</span><span class="sxs-lookup"><span data-stu-id="d5117-124">Type</span></span>   | <span data-ttu-id="d5117-125">说明</span><span class="sxs-lookup"><span data-stu-id="d5117-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d5117-126">period</span><span class="sxs-lookup"><span data-stu-id="d5117-126">period</span></span>    | <span data-ttu-id="d5117-127">string</span><span class="sxs-lookup"><span data-stu-id="d5117-127">string</span></span> | <span data-ttu-id="d5117-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d5117-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d5117-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d5117-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d5117-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d5117-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d5117-131">date</span><span class="sxs-lookup"><span data-stu-id="d5117-131">date</span></span>      | <span data-ttu-id="d5117-132">Date</span><span class="sxs-lookup"><span data-stu-id="d5117-132">Date</span></span>   | <span data-ttu-id="d5117-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="d5117-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d5117-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="d5117-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d5117-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="d5117-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d5117-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="d5117-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="d5117-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d5117-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d5117-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="d5117-138">The default output type is text/csv.</span></span> <span data-ttu-id="d5117-139">但是，如果要指定输出类型，可以使用设置为 text/csv 或 application/json 的 OData $format查询参数。</span><span class="sxs-lookup"><span data-stu-id="d5117-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5117-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5117-140">Request headers</span></span>

| <span data-ttu-id="d5117-141">名称</span><span class="sxs-lookup"><span data-stu-id="d5117-141">Name</span></span>          | <span data-ttu-id="d5117-142">说明</span><span class="sxs-lookup"><span data-stu-id="d5117-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d5117-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5117-143">Authorization</span></span> | <span data-ttu-id="d5117-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5117-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d5117-146">响应</span><span class="sxs-lookup"><span data-stu-id="d5117-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d5117-147">CSV</span><span class="sxs-lookup"><span data-stu-id="d5117-147">CSV</span></span>

<span data-ttu-id="d5117-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d5117-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d5117-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d5117-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d5117-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d5117-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d5117-151">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d5117-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d5117-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d5117-152">Report Refresh Date</span></span>
- <span data-ttu-id="d5117-153">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d5117-153">User Principal Name</span></span>
- <span data-ttu-id="d5117-154">已删除</span><span class="sxs-lookup"><span data-stu-id="d5117-154">Is Deleted</span></span>
- <span data-ttu-id="d5117-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="d5117-155">Deleted Date</span></span>
- <span data-ttu-id="d5117-156">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="d5117-156">Last Activity Date</span></span>
- <span data-ttu-id="d5117-157">已查看或编辑文件数</span><span class="sxs-lookup"><span data-stu-id="d5117-157">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="d5117-158">已同步文件数</span><span class="sxs-lookup"><span data-stu-id="d5117-158">Synced File Count</span></span>
- <span data-ttu-id="d5117-159">已内部共享文件数</span><span class="sxs-lookup"><span data-stu-id="d5117-159">Shared Internally File Count</span></span>
- <span data-ttu-id="d5117-160">已外部共享文件数</span><span class="sxs-lookup"><span data-stu-id="d5117-160">Shared Externally File Count</span></span>
- <span data-ttu-id="d5117-161">分配的产品</span><span class="sxs-lookup"><span data-stu-id="d5117-161">Assigned Products</span></span>
- <span data-ttu-id="d5117-162">报表周期</span><span class="sxs-lookup"><span data-stu-id="d5117-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d5117-163">JSON</span><span class="sxs-lookup"><span data-stu-id="d5117-163">JSON</span></span>

<span data-ttu-id="d5117-164">如果成功，此方法在响应正文中返回响应代码和 `200 OK` **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="d5117-164">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="d5117-165">此请求的默认页面大小为 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="d5117-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="d5117-166">示例</span><span class="sxs-lookup"><span data-stu-id="d5117-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d5117-167">CSV</span><span class="sxs-lookup"><span data-stu-id="d5117-167">CSV</span></span>

<span data-ttu-id="d5117-168">下面是一个输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="d5117-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d5117-169">请求</span><span class="sxs-lookup"><span data-stu-id="d5117-169">Request</span></span>

<span data-ttu-id="d5117-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d5117-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="d5117-171">响应</span><span class="sxs-lookup"><span data-stu-id="d5117-171">Response</span></span>

<span data-ttu-id="d5117-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d5117-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d5117-173">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d5117-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Viewed Or Edited File Count,Synced File Count,Shared Internally File Count,Shared Externally File Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="d5117-174">JSON</span><span class="sxs-lookup"><span data-stu-id="d5117-174">JSON</span></span>

<span data-ttu-id="d5117-175">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d5117-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d5117-176">请求</span><span class="sxs-lookup"><span data-stu-id="d5117-176">Request</span></span>

<span data-ttu-id="d5117-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d5117-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="d5117-178">响应</span><span class="sxs-lookup"><span data-stu-id="d5117-178">Response</span></span>

<span data-ttu-id="d5117-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d5117-179">The following is an example of the response.</span></span>

> <span data-ttu-id="d5117-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d5117-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "viewedOrEditedFileCount": 1, 
      "syncedFileCount": 0, 
      "sharedInternallyFileCount": 0, 
      "sharedExternallyFileCount": 0, 
      "assignedProducts": [
        "Microsoft 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


