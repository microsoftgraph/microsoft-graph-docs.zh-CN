---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: 获取组执行的 Yammer 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a8df675d76f554fc61737cc49942652772650f97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545553"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="ca2a9-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="ca2a9-103">reportRoot: getYammerGroupsActivityDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca2a9-104">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="ca2a9-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca2a9-106">权限</span><span class="sxs-lookup"><span data-stu-id="ca2a9-106">Permissions</span></span>

<span data-ttu-id="ca2a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca2a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca2a9-109">Permission type</span></span>                        | <span data-ttu-id="ca2a9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca2a9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ca2a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca2a9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca2a9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca2a9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ca2a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca2a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca2a9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-114">Not supported.</span></span>                           |
| <span data-ttu-id="ca2a9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca2a9-115">Application</span></span>                            | <span data-ttu-id="ca2a9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca2a9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ca2a9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca2a9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ca2a9-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="ca2a9-118">Function parameters</span></span>

<span data-ttu-id="ca2a9-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ca2a9-120">参数</span><span class="sxs-lookup"><span data-stu-id="ca2a9-120">Parameter</span></span> | <span data-ttu-id="ca2a9-121">类型</span><span class="sxs-lookup"><span data-stu-id="ca2a9-121">Type</span></span>   | <span data-ttu-id="ca2a9-122">说明</span><span class="sxs-lookup"><span data-stu-id="ca2a9-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ca2a9-123">period</span><span class="sxs-lookup"><span data-stu-id="ca2a9-123">period</span></span>    | <span data-ttu-id="ca2a9-124">string</span><span class="sxs-lookup"><span data-stu-id="ca2a9-124">string</span></span> | <span data-ttu-id="ca2a9-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ca2a9-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ca2a9-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ca2a9-128">date</span><span class="sxs-lookup"><span data-stu-id="ca2a9-128">date</span></span>      | <span data-ttu-id="ca2a9-129">Date</span><span class="sxs-lookup"><span data-stu-id="ca2a9-129">Date</span></span>   | <span data-ttu-id="ca2a9-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ca2a9-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ca2a9-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ca2a9-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="ca2a9-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ca2a9-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-135">The default output type is text/csv.</span></span> <span data-ttu-id="ca2a9-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca2a9-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca2a9-137">Request headers</span></span>

| <span data-ttu-id="ca2a9-138">名称</span><span class="sxs-lookup"><span data-stu-id="ca2a9-138">Name</span></span>          | <span data-ttu-id="ca2a9-139">说明</span><span class="sxs-lookup"><span data-stu-id="ca2a9-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ca2a9-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca2a9-140">Authorization</span></span> | <span data-ttu-id="ca2a9-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ca2a9-143">响应</span><span class="sxs-lookup"><span data-stu-id="ca2a9-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ca2a9-144">CSV</span><span class="sxs-lookup"><span data-stu-id="ca2a9-144">CSV</span></span>

<span data-ttu-id="ca2a9-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ca2a9-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ca2a9-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ca2a9-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ca2a9-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ca2a9-149">Report Refresh Date</span></span>
- <span data-ttu-id="ca2a9-150">组显示名称</span><span class="sxs-lookup"><span data-stu-id="ca2a9-150">Group Display Name</span></span>
- <span data-ttu-id="ca2a9-151">已删除</span><span class="sxs-lookup"><span data-stu-id="ca2a9-151">Is Deleted</span></span>
- <span data-ttu-id="ca2a9-152">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="ca2a9-152">Owner Principal Name</span></span>
- <span data-ttu-id="ca2a9-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="ca2a9-153">Last Activity Date</span></span>
- <span data-ttu-id="ca2a9-154">组类型</span><span class="sxs-lookup"><span data-stu-id="ca2a9-154">Group Type</span></span>
- <span data-ttu-id="ca2a9-155">Office 365 已连接</span><span class="sxs-lookup"><span data-stu-id="ca2a9-155">Office 365 Connected</span></span>
- <span data-ttu-id="ca2a9-156">成员数</span><span class="sxs-lookup"><span data-stu-id="ca2a9-156">Member Count</span></span>
- <span data-ttu-id="ca2a9-157">已发布数</span><span class="sxs-lookup"><span data-stu-id="ca2a9-157">Posted Count</span></span>
- <span data-ttu-id="ca2a9-158">已阅读数</span><span class="sxs-lookup"><span data-stu-id="ca2a9-158">Read Count</span></span>
- <span data-ttu-id="ca2a9-159">已赞数</span><span class="sxs-lookup"><span data-stu-id="ca2a9-159">Liked Count</span></span>
- <span data-ttu-id="ca2a9-160">报表周期</span><span class="sxs-lookup"><span data-stu-id="ca2a9-160">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ca2a9-161">JSON</span><span class="sxs-lookup"><span data-stu-id="ca2a9-161">JSON</span></span>

<span data-ttu-id="ca2a9-162">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-162">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="ca2a9-163">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-163">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="ca2a9-164">示例</span><span class="sxs-lookup"><span data-stu-id="ca2a9-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ca2a9-165">CSV</span><span class="sxs-lookup"><span data-stu-id="ca2a9-165">CSV</span></span>

<span data-ttu-id="ca2a9-166">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ca2a9-167">请求</span><span class="sxs-lookup"><span data-stu-id="ca2a9-167">Request</span></span>

<span data-ttu-id="ca2a9-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="ca2a9-169">响应</span><span class="sxs-lookup"><span data-stu-id="ca2a9-169">Response</span></span>

<span data-ttu-id="ca2a9-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-170">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ca2a9-171">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-171">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="ca2a9-172">JSON</span><span class="sxs-lookup"><span data-stu-id="ca2a9-172">JSON</span></span>

<span data-ttu-id="ca2a9-173">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-173">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ca2a9-174">请求</span><span class="sxs-lookup"><span data-stu-id="ca2a9-174">Request</span></span>

<span data-ttu-id="ca2a9-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="ca2a9-176">响应</span><span class="sxs-lookup"><span data-stu-id="ca2a9-176">Response</span></span>

<span data-ttu-id="ca2a9-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-177">The following is an example of the response.</span></span>

> <span data-ttu-id="ca2a9-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ca2a9-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
      "reportPeriod": "7"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitydetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
