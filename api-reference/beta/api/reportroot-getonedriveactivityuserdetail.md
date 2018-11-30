---
title: 'reportRoot: getOneDriveActivityUserDetail'
description: 获取用户执行的 OneDrive 活动的详细信息。
ms.openlocfilehash: b992960a366ba6b8596b8b276abcd88afb5e8855
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043084"
---
# <a name="reportroot-getonedriveactivityuserdetail"></a><span data-ttu-id="9ed99-103">reportRoot: getOneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="9ed99-103">reportRoot: getOneDriveActivityUserDetail</span></span>

> <span data-ttu-id="9ed99-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9ed99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ed99-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ed99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ed99-106">获取用户执行的 OneDrive 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9ed99-106">Get details about OneDrive activity by user.</span></span>

> <span data-ttu-id="9ed99-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="9ed99-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ed99-108">权限</span><span class="sxs-lookup"><span data-stu-id="9ed99-108">Permissions</span></span>

<span data-ttu-id="9ed99-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ed99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ed99-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ed99-111">Permission type</span></span>                        | <span data-ttu-id="9ed99-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ed99-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="9ed99-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ed99-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ed99-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ed99-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="9ed99-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ed99-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed99-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ed99-116">Not supported.</span></span>                           |
| <span data-ttu-id="9ed99-117">应用</span><span class="sxs-lookup"><span data-stu-id="9ed99-117">Application</span></span>                            | <span data-ttu-id="9ed99-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ed99-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="9ed99-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ed99-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserDetail(period='{period_value}')
GET /reports/getOneDriveActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="9ed99-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="9ed99-120">Function parameters</span></span>

<span data-ttu-id="9ed99-121">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="9ed99-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="9ed99-122">参数</span><span class="sxs-lookup"><span data-stu-id="9ed99-122">Parameter</span></span> | <span data-ttu-id="9ed99-123">类型</span><span class="sxs-lookup"><span data-stu-id="9ed99-123">Type</span></span>   | <span data-ttu-id="9ed99-124">说明</span><span class="sxs-lookup"><span data-stu-id="9ed99-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="9ed99-125">period</span><span class="sxs-lookup"><span data-stu-id="9ed99-125">period</span></span>    | <span data-ttu-id="9ed99-126">string</span><span class="sxs-lookup"><span data-stu-id="9ed99-126">string</span></span> | <span data-ttu-id="9ed99-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9ed99-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="9ed99-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="9ed99-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="9ed99-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="9ed99-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="9ed99-130">date</span><span class="sxs-lookup"><span data-stu-id="9ed99-130">date</span></span>      | <span data-ttu-id="9ed99-131">Date</span><span class="sxs-lookup"><span data-stu-id="9ed99-131">Date</span></span>   | <span data-ttu-id="9ed99-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="9ed99-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="9ed99-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="9ed99-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="9ed99-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="9ed99-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="9ed99-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="9ed99-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="9ed99-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9ed99-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="9ed99-137">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="9ed99-137">The default output type is text/csv.</span></span> <span data-ttu-id="9ed99-138">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="9ed99-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ed99-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ed99-139">Request headers</span></span>

| <span data-ttu-id="9ed99-140">名称</span><span class="sxs-lookup"><span data-stu-id="9ed99-140">Name</span></span>          | <span data-ttu-id="9ed99-141">说明</span><span class="sxs-lookup"><span data-stu-id="9ed99-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="9ed99-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ed99-142">Authorization</span></span> | <span data-ttu-id="9ed99-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ed99-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="9ed99-145">响应</span><span class="sxs-lookup"><span data-stu-id="9ed99-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="9ed99-146">CSV</span><span class="sxs-lookup"><span data-stu-id="9ed99-146">CSV</span></span>

<span data-ttu-id="9ed99-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="9ed99-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="9ed99-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="9ed99-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="9ed99-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="9ed99-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="9ed99-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="9ed99-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="9ed99-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="9ed99-151">Report Refresh Date</span></span>
- <span data-ttu-id="9ed99-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="9ed99-152">User Principal Name</span></span>
- <span data-ttu-id="9ed99-153">已删除</span><span class="sxs-lookup"><span data-stu-id="9ed99-153">Is Deleted</span></span>
- <span data-ttu-id="9ed99-154">删除日期</span><span class="sxs-lookup"><span data-stu-id="9ed99-154">Deleted Date</span></span>
- <span data-ttu-id="9ed99-155">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="9ed99-155">Last Activity Date</span></span>
- <span data-ttu-id="9ed99-156">已查看或编辑文件数</span><span class="sxs-lookup"><span data-stu-id="9ed99-156">Viewed Or Edited File Count</span></span>
- <span data-ttu-id="9ed99-157">已同步文件数</span><span class="sxs-lookup"><span data-stu-id="9ed99-157">Synced File Count</span></span>
- <span data-ttu-id="9ed99-158">已内部共享文件数</span><span class="sxs-lookup"><span data-stu-id="9ed99-158">Shared Internally File Count</span></span>
- <span data-ttu-id="9ed99-159">已外部共享文件数</span><span class="sxs-lookup"><span data-stu-id="9ed99-159">Shared Externally File Count</span></span>
- <span data-ttu-id="9ed99-160">分配的产品</span><span class="sxs-lookup"><span data-stu-id="9ed99-160">Assigned Products</span></span>
- <span data-ttu-id="9ed99-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="9ed99-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="9ed99-162">JSON</span><span class="sxs-lookup"><span data-stu-id="9ed99-162">JSON</span></span>

<span data-ttu-id="9ed99-163">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="9ed99-163">If successful, this method returns a `200 OK` response code and a **[oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="9ed99-164">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="9ed99-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="9ed99-165">示例</span><span class="sxs-lookup"><span data-stu-id="9ed99-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="9ed99-166">CSV</span><span class="sxs-lookup"><span data-stu-id="9ed99-166">CSV</span></span>

<span data-ttu-id="9ed99-167">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="9ed99-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="9ed99-168">请求</span><span class="sxs-lookup"><span data-stu-id="9ed99-168">Request</span></span>

<span data-ttu-id="9ed99-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed99-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="9ed99-170">响应</span><span class="sxs-lookup"><span data-stu-id="9ed99-170">Response</span></span>

<span data-ttu-id="9ed99-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed99-171">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="9ed99-172">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="9ed99-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="9ed99-173">JSON</span><span class="sxs-lookup"><span data-stu-id="9ed99-173">JSON</span></span>

<span data-ttu-id="9ed99-174">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="9ed99-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="9ed99-175">请求</span><span class="sxs-lookup"><span data-stu-id="9ed99-175">Request</span></span>

<span data-ttu-id="9ed99-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ed99-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="9ed99-177">响应</span><span class="sxs-lookup"><span data-stu-id="9ed99-177">Response</span></span>

<span data-ttu-id="9ed99-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ed99-178">The following is an example of the response.</span></span>

> <span data-ttu-id="9ed99-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9ed99-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "reportPeriod": "7"
    }
  ]
}
```
