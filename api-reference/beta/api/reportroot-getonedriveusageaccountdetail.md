---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: 获取帐户的 OneDrive 使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 51fe0d89b8ad4e8bb783c901fba101135a296834
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525750"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="b6c1f-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="b6c1f-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6c1f-104">获取帐户的 OneDrive 使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="b6c1f-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6c1f-106">权限</span><span class="sxs-lookup"><span data-stu-id="b6c1f-106">Permissions</span></span>

<span data-ttu-id="b6c1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b6c1f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6c1f-109">Permission type</span></span>                        | <span data-ttu-id="b6c1f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b6c1f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b6c1f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6c1f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b6c1f-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c1f-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b6c1f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6c1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6c1f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-114">Not supported.</span></span>                           |
| <span data-ttu-id="b6c1f-115">应用</span><span class="sxs-lookup"><span data-stu-id="b6c1f-115">Application</span></span>                            | <span data-ttu-id="b6c1f-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c1f-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b6c1f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6c1f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b6c1f-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="b6c1f-118">Function parameters</span></span>

<span data-ttu-id="b6c1f-119">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b6c1f-120">参数</span><span class="sxs-lookup"><span data-stu-id="b6c1f-120">Parameter</span></span> | <span data-ttu-id="b6c1f-121">类型</span><span class="sxs-lookup"><span data-stu-id="b6c1f-121">Type</span></span>   | <span data-ttu-id="b6c1f-122">说明</span><span class="sxs-lookup"><span data-stu-id="b6c1f-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b6c1f-123">period</span><span class="sxs-lookup"><span data-stu-id="b6c1f-123">period</span></span>    | <span data-ttu-id="b6c1f-124">string</span><span class="sxs-lookup"><span data-stu-id="b6c1f-124">string</span></span> | <span data-ttu-id="b6c1f-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b6c1f-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b6c1f-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b6c1f-128">date</span><span class="sxs-lookup"><span data-stu-id="b6c1f-128">date</span></span>      | <span data-ttu-id="b6c1f-129">Date</span><span class="sxs-lookup"><span data-stu-id="b6c1f-129">Date</span></span>   | <span data-ttu-id="b6c1f-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b6c1f-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b6c1f-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b6c1f-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="b6c1f-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b6c1f-135">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-135">The default output type is text/csv.</span></span> <span data-ttu-id="b6c1f-136">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6c1f-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6c1f-137">Request headers</span></span>

| <span data-ttu-id="b6c1f-138">名称</span><span class="sxs-lookup"><span data-stu-id="b6c1f-138">Name</span></span>          | <span data-ttu-id="b6c1f-139">说明</span><span class="sxs-lookup"><span data-stu-id="b6c1f-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b6c1f-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6c1f-140">Authorization</span></span> | <span data-ttu-id="b6c1f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b6c1f-143">响应</span><span class="sxs-lookup"><span data-stu-id="b6c1f-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b6c1f-144">CSV</span><span class="sxs-lookup"><span data-stu-id="b6c1f-144">CSV</span></span>

<span data-ttu-id="b6c1f-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b6c1f-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b6c1f-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b6c1f-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b6c1f-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b6c1f-149">Report Refresh Date</span></span>
- <span data-ttu-id="b6c1f-150">网站 URL</span><span class="sxs-lookup"><span data-stu-id="b6c1f-150">Site URL</span></span>
- <span data-ttu-id="b6c1f-151">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="b6c1f-151">Owner Display Name</span></span>
- <span data-ttu-id="b6c1f-152">已删除</span><span class="sxs-lookup"><span data-stu-id="b6c1f-152">Is Deleted</span></span>
- <span data-ttu-id="b6c1f-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="b6c1f-153">Last Activity Date</span></span>
- <span data-ttu-id="b6c1f-154">文件数</span><span class="sxs-lookup"><span data-stu-id="b6c1f-154">File Count</span></span>
- <span data-ttu-id="b6c1f-155">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="b6c1f-155">Active File Count</span></span>
- <span data-ttu-id="b6c1f-156">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="b6c1f-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="b6c1f-157">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="b6c1f-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="b6c1f-158">报表周期</span><span class="sxs-lookup"><span data-stu-id="b6c1f-158">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="b6c1f-159">JSON</span><span class="sxs-lookup"><span data-stu-id="b6c1f-159">JSON</span></span>

<span data-ttu-id="b6c1f-160">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-160">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="b6c1f-161">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-161">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="b6c1f-162">示例</span><span class="sxs-lookup"><span data-stu-id="b6c1f-162">Example</span></span>

<span data-ttu-id="b6c1f-163">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-163">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="b6c1f-164">CSV</span><span class="sxs-lookup"><span data-stu-id="b6c1f-164">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="b6c1f-165">请求</span><span class="sxs-lookup"><span data-stu-id="b6c1f-165">Request</span></span>

<span data-ttu-id="b6c1f-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="b6c1f-167">响应</span><span class="sxs-lookup"><span data-stu-id="b6c1f-167">Response</span></span>

<span data-ttu-id="b6c1f-168">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b6c1f-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="b6c1f-170">JSON</span><span class="sxs-lookup"><span data-stu-id="b6c1f-170">JSON</span></span>

<span data-ttu-id="b6c1f-171">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b6c1f-172">请求</span><span class="sxs-lookup"><span data-stu-id="b6c1f-172">Request</span></span>

<span data-ttu-id="b6c1f-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="b6c1f-174">响应</span><span class="sxs-lookup"><span data-stu-id="b6c1f-174">Response</span></span>

<span data-ttu-id="b6c1f-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-175">The following is an example of the response.</span></span>

> <span data-ttu-id="b6c1f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b6c1f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
