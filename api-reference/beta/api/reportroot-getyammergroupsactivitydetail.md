---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: 获取组执行的 Yammer 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d589f6b8d9a5e51fe77c7da13ce3c5c0f662acce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942876"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="905bb-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="905bb-103">reportRoot: getYammerGroupsActivityDetail</span></span>

> <span data-ttu-id="905bb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="905bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="905bb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="905bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="905bb-106">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="905bb-106">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="905bb-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="905bb-107">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="905bb-108">权限</span><span class="sxs-lookup"><span data-stu-id="905bb-108">Permissions</span></span>

<span data-ttu-id="905bb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="905bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="905bb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="905bb-111">Permission type</span></span>                        | <span data-ttu-id="905bb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="905bb-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="905bb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="905bb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="905bb-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="905bb-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="905bb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="905bb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="905bb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="905bb-116">Not supported.</span></span>                           |
| <span data-ttu-id="905bb-117">应用</span><span class="sxs-lookup"><span data-stu-id="905bb-117">Application</span></span>                            | <span data-ttu-id="905bb-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="905bb-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="905bb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="905bb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="905bb-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="905bb-120">Function parameters</span></span>

<span data-ttu-id="905bb-121">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="905bb-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="905bb-122">参数</span><span class="sxs-lookup"><span data-stu-id="905bb-122">Parameter</span></span> | <span data-ttu-id="905bb-123">类型</span><span class="sxs-lookup"><span data-stu-id="905bb-123">Type</span></span>   | <span data-ttu-id="905bb-124">说明</span><span class="sxs-lookup"><span data-stu-id="905bb-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="905bb-125">period</span><span class="sxs-lookup"><span data-stu-id="905bb-125">period</span></span>    | <span data-ttu-id="905bb-126">string</span><span class="sxs-lookup"><span data-stu-id="905bb-126">string</span></span> | <span data-ttu-id="905bb-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="905bb-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="905bb-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="905bb-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="905bb-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="905bb-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="905bb-130">date</span><span class="sxs-lookup"><span data-stu-id="905bb-130">date</span></span>      | <span data-ttu-id="905bb-131">Date</span><span class="sxs-lookup"><span data-stu-id="905bb-131">Date</span></span>   | <span data-ttu-id="905bb-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="905bb-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="905bb-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="905bb-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="905bb-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="905bb-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="905bb-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="905bb-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="905bb-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="905bb-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="905bb-137">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="905bb-137">The default output type is text/csv.</span></span> <span data-ttu-id="905bb-138">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="905bb-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="905bb-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="905bb-139">Request headers</span></span>

| <span data-ttu-id="905bb-140">名称</span><span class="sxs-lookup"><span data-stu-id="905bb-140">Name</span></span>          | <span data-ttu-id="905bb-141">说明</span><span class="sxs-lookup"><span data-stu-id="905bb-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="905bb-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="905bb-142">Authorization</span></span> | <span data-ttu-id="905bb-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="905bb-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="905bb-145">响应</span><span class="sxs-lookup"><span data-stu-id="905bb-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="905bb-146">CSV</span><span class="sxs-lookup"><span data-stu-id="905bb-146">CSV</span></span>

<span data-ttu-id="905bb-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="905bb-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="905bb-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="905bb-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="905bb-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="905bb-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="905bb-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="905bb-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="905bb-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="905bb-151">Report Refresh Date</span></span>
- <span data-ttu-id="905bb-152">组显示名称</span><span class="sxs-lookup"><span data-stu-id="905bb-152">Group Display Name</span></span>
- <span data-ttu-id="905bb-153">已删除</span><span class="sxs-lookup"><span data-stu-id="905bb-153">Is Deleted</span></span>
- <span data-ttu-id="905bb-154">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="905bb-154">Owner Principal Name</span></span>
- <span data-ttu-id="905bb-155">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="905bb-155">Last Activity Date</span></span>
- <span data-ttu-id="905bb-156">组类型</span><span class="sxs-lookup"><span data-stu-id="905bb-156">Group Type</span></span>
- <span data-ttu-id="905bb-157">Office 365 已连接</span><span class="sxs-lookup"><span data-stu-id="905bb-157">Office 365 Connected</span></span>
- <span data-ttu-id="905bb-158">成员数</span><span class="sxs-lookup"><span data-stu-id="905bb-158">Member Count</span></span>
- <span data-ttu-id="905bb-159">已发布数</span><span class="sxs-lookup"><span data-stu-id="905bb-159">Posted Count</span></span>
- <span data-ttu-id="905bb-160">已阅读数</span><span class="sxs-lookup"><span data-stu-id="905bb-160">Read Count</span></span>
- <span data-ttu-id="905bb-161">已赞数</span><span class="sxs-lookup"><span data-stu-id="905bb-161">Liked Count</span></span>
- <span data-ttu-id="905bb-162">报表周期</span><span class="sxs-lookup"><span data-stu-id="905bb-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="905bb-163">JSON</span><span class="sxs-lookup"><span data-stu-id="905bb-163">JSON</span></span>

<span data-ttu-id="905bb-164">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="905bb-164">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="905bb-165">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="905bb-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="905bb-166">示例</span><span class="sxs-lookup"><span data-stu-id="905bb-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="905bb-167">CSV</span><span class="sxs-lookup"><span data-stu-id="905bb-167">CSV</span></span>

<span data-ttu-id="905bb-168">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="905bb-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="905bb-169">请求</span><span class="sxs-lookup"><span data-stu-id="905bb-169">Request</span></span>

<span data-ttu-id="905bb-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="905bb-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="905bb-171">响应</span><span class="sxs-lookup"><span data-stu-id="905bb-171">Response</span></span>

<span data-ttu-id="905bb-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="905bb-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="905bb-173">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="905bb-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="905bb-174">JSON</span><span class="sxs-lookup"><span data-stu-id="905bb-174">JSON</span></span>

<span data-ttu-id="905bb-175">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="905bb-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="905bb-176">请求</span><span class="sxs-lookup"><span data-stu-id="905bb-176">Request</span></span>

<span data-ttu-id="905bb-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="905bb-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="905bb-178">响应</span><span class="sxs-lookup"><span data-stu-id="905bb-178">Response</span></span>

<span data-ttu-id="905bb-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="905bb-179">The following is an example of the response.</span></span>

> <span data-ttu-id="905bb-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="905bb-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
