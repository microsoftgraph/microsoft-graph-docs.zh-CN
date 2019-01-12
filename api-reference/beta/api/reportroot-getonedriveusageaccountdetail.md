---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: 获取帐户的 OneDrive 使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 1aa7de008f1791908786111a87c1ab046df7f42e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960299"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="63f15-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="63f15-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

> <span data-ttu-id="63f15-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="63f15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63f15-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63f15-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63f15-106">获取帐户的 OneDrive 使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="63f15-106">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="63f15-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="63f15-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="63f15-108">权限</span><span class="sxs-lookup"><span data-stu-id="63f15-108">Permissions</span></span>

<span data-ttu-id="63f15-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63f15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63f15-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="63f15-111">Permission type</span></span>                        | <span data-ttu-id="63f15-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63f15-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="63f15-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63f15-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="63f15-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63f15-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="63f15-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63f15-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63f15-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63f15-116">Not supported.</span></span>                           |
| <span data-ttu-id="63f15-117">应用</span><span class="sxs-lookup"><span data-stu-id="63f15-117">Application</span></span>                            | <span data-ttu-id="63f15-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="63f15-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="63f15-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63f15-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="63f15-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="63f15-120">Function parameters</span></span>

<span data-ttu-id="63f15-121">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="63f15-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="63f15-122">参数</span><span class="sxs-lookup"><span data-stu-id="63f15-122">Parameter</span></span> | <span data-ttu-id="63f15-123">类型</span><span class="sxs-lookup"><span data-stu-id="63f15-123">Type</span></span>   | <span data-ttu-id="63f15-124">说明</span><span class="sxs-lookup"><span data-stu-id="63f15-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="63f15-125">period</span><span class="sxs-lookup"><span data-stu-id="63f15-125">period</span></span>    | <span data-ttu-id="63f15-126">string</span><span class="sxs-lookup"><span data-stu-id="63f15-126">string</span></span> | <span data-ttu-id="63f15-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="63f15-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="63f15-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="63f15-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="63f15-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="63f15-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="63f15-130">date</span><span class="sxs-lookup"><span data-stu-id="63f15-130">date</span></span>      | <span data-ttu-id="63f15-131">Date</span><span class="sxs-lookup"><span data-stu-id="63f15-131">Date</span></span>   | <span data-ttu-id="63f15-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="63f15-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="63f15-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="63f15-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="63f15-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="63f15-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="63f15-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="63f15-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="63f15-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="63f15-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="63f15-137">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="63f15-137">The default output type is text/csv.</span></span> <span data-ttu-id="63f15-138">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="63f15-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63f15-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="63f15-139">Request headers</span></span>

| <span data-ttu-id="63f15-140">名称</span><span class="sxs-lookup"><span data-stu-id="63f15-140">Name</span></span>          | <span data-ttu-id="63f15-141">说明</span><span class="sxs-lookup"><span data-stu-id="63f15-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="63f15-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="63f15-142">Authorization</span></span> | <span data-ttu-id="63f15-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63f15-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="63f15-145">响应</span><span class="sxs-lookup"><span data-stu-id="63f15-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="63f15-146">CSV</span><span class="sxs-lookup"><span data-stu-id="63f15-146">CSV</span></span>

<span data-ttu-id="63f15-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="63f15-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="63f15-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="63f15-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="63f15-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="63f15-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="63f15-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="63f15-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="63f15-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="63f15-151">Report Refresh Date</span></span>
- <span data-ttu-id="63f15-152">网站 URL</span><span class="sxs-lookup"><span data-stu-id="63f15-152">Site URL</span></span>
- <span data-ttu-id="63f15-153">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="63f15-153">Owner Display Name</span></span>
- <span data-ttu-id="63f15-154">已删除</span><span class="sxs-lookup"><span data-stu-id="63f15-154">Is Deleted</span></span>
- <span data-ttu-id="63f15-155">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="63f15-155">Last Activity Date</span></span>
- <span data-ttu-id="63f15-156">文件数</span><span class="sxs-lookup"><span data-stu-id="63f15-156">File Count</span></span>
- <span data-ttu-id="63f15-157">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="63f15-157">Active File Count</span></span>
- <span data-ttu-id="63f15-158">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="63f15-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="63f15-159">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="63f15-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="63f15-160">报表周期</span><span class="sxs-lookup"><span data-stu-id="63f15-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="63f15-161">JSON</span><span class="sxs-lookup"><span data-stu-id="63f15-161">JSON</span></span>

<span data-ttu-id="63f15-162">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="63f15-162">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="63f15-163">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="63f15-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="63f15-164">示例</span><span class="sxs-lookup"><span data-stu-id="63f15-164">Example</span></span>

<span data-ttu-id="63f15-165">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="63f15-165">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="63f15-166">CSV</span><span class="sxs-lookup"><span data-stu-id="63f15-166">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="63f15-167">请求</span><span class="sxs-lookup"><span data-stu-id="63f15-167">Request</span></span>

<span data-ttu-id="63f15-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63f15-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="63f15-169">响应</span><span class="sxs-lookup"><span data-stu-id="63f15-169">Response</span></span>

<span data-ttu-id="63f15-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63f15-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="63f15-171">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="63f15-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Report Period
```

### <a name="json"></a><span data-ttu-id="63f15-172">JSON</span><span class="sxs-lookup"><span data-stu-id="63f15-172">JSON</span></span>

<span data-ttu-id="63f15-173">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="63f15-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="63f15-174">请求</span><span class="sxs-lookup"><span data-stu-id="63f15-174">Request</span></span>

<span data-ttu-id="63f15-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63f15-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="63f15-176">响应</span><span class="sxs-lookup"><span data-stu-id="63f15-176">Response</span></span>

<span data-ttu-id="63f15-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63f15-177">The following is an example of the response.</span></span>

> <span data-ttu-id="63f15-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="63f15-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
      "reportPeriod": "7"
    }
  ]
}
```
