---
title: 'reportRoot: getYammerActivityUserDetail'
description: 获取用户执行的 Yammer 活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 72fa1512077b40ac48f5912b4bb22ef895a4912b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982857"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="ad861-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ad861-103">reportRoot: getYammerActivityUserDetail</span></span>

<span data-ttu-id="ad861-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad861-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad861-105">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ad861-105">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="ad861-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="ad861-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="ad861-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ad861-107">Permissions</span></span>

<span data-ttu-id="ad861-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad861-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ad861-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad861-110">Permission type</span></span>                        | <span data-ttu-id="ad861-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad861-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="ad861-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad861-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ad861-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad861-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="ad861-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad861-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad861-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad861-115">Not supported.</span></span>                           |
| <span data-ttu-id="ad861-116">应用</span><span class="sxs-lookup"><span data-stu-id="ad861-116">Application</span></span>                            | <span data-ttu-id="ad861-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad861-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="ad861-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="ad861-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="ad861-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="ad861-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="ad861-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad861-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="ad861-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="ad861-121">Function parameters</span></span>

<span data-ttu-id="ad861-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="ad861-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="ad861-123">参数</span><span class="sxs-lookup"><span data-stu-id="ad861-123">Parameter</span></span> | <span data-ttu-id="ad861-124">类型</span><span class="sxs-lookup"><span data-stu-id="ad861-124">Type</span></span>   | <span data-ttu-id="ad861-125">说明</span><span class="sxs-lookup"><span data-stu-id="ad861-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="ad861-126">period</span><span class="sxs-lookup"><span data-stu-id="ad861-126">period</span></span>    | <span data-ttu-id="ad861-127">string</span><span class="sxs-lookup"><span data-stu-id="ad861-127">string</span></span> | <span data-ttu-id="ad861-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ad861-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="ad861-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="ad861-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="ad861-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="ad861-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="ad861-131">date</span><span class="sxs-lookup"><span data-stu-id="ad861-131">date</span></span>      | <span data-ttu-id="ad861-132">Date</span><span class="sxs-lookup"><span data-stu-id="ad861-132">Date</span></span>   | <span data-ttu-id="ad861-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="ad861-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="ad861-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="ad861-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="ad861-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="ad861-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="ad861-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="ad861-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="ad861-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ad861-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="ad861-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="ad861-138">The default output type is text/csv.</span></span> <span data-ttu-id="ad861-139">但是，如果要指定输出类型，可以使用设置为 text/csv 或 application/json 的 OData $format查询参数。</span><span class="sxs-lookup"><span data-stu-id="ad861-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad861-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad861-140">Request headers</span></span>

| <span data-ttu-id="ad861-141">名称</span><span class="sxs-lookup"><span data-stu-id="ad861-141">Name</span></span>          | <span data-ttu-id="ad861-142">说明</span><span class="sxs-lookup"><span data-stu-id="ad861-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="ad861-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad861-143">Authorization</span></span> | <span data-ttu-id="ad861-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ad861-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="ad861-146">响应</span><span class="sxs-lookup"><span data-stu-id="ad861-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="ad861-147">CSV</span><span class="sxs-lookup"><span data-stu-id="ad861-147">CSV</span></span>

<span data-ttu-id="ad861-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="ad861-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="ad861-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="ad861-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="ad861-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="ad861-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="ad861-151">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="ad861-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="ad861-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="ad861-152">Report Refresh Date</span></span>
- <span data-ttu-id="ad861-153">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="ad861-153">User Principal Name</span></span>
- <span data-ttu-id="ad861-154">显示名称</span><span class="sxs-lookup"><span data-stu-id="ad861-154">Display Name</span></span>
- <span data-ttu-id="ad861-155">用户状态</span><span class="sxs-lookup"><span data-stu-id="ad861-155">User State</span></span>
- <span data-ttu-id="ad861-156">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="ad861-156">State Change Date</span></span>
- <span data-ttu-id="ad861-157">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="ad861-157">Last Activity Date</span></span>
- <span data-ttu-id="ad861-158">已发布数</span><span class="sxs-lookup"><span data-stu-id="ad861-158">Posted Count</span></span>
- <span data-ttu-id="ad861-159">已阅读数</span><span class="sxs-lookup"><span data-stu-id="ad861-159">Read Count</span></span>
- <span data-ttu-id="ad861-160">已赞数</span><span class="sxs-lookup"><span data-stu-id="ad861-160">Liked Count</span></span>
- <span data-ttu-id="ad861-161">分配的产品</span><span class="sxs-lookup"><span data-stu-id="ad861-161">Assigned Products</span></span>
- <span data-ttu-id="ad861-162">报表周期</span><span class="sxs-lookup"><span data-stu-id="ad861-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="ad861-163">JSON</span><span class="sxs-lookup"><span data-stu-id="ad861-163">JSON</span></span>

<span data-ttu-id="ad861-164">如果成功，此方法在响应正文中返回响应代码和 `200 OK` **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="ad861-164">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="ad861-165">此请求的默认页面大小为 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="ad861-165">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="ad861-166">示例</span><span class="sxs-lookup"><span data-stu-id="ad861-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="ad861-167">CSV</span><span class="sxs-lookup"><span data-stu-id="ad861-167">CSV</span></span>

<span data-ttu-id="ad861-168">下面是一个输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="ad861-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="ad861-169">请求</span><span class="sxs-lookup"><span data-stu-id="ad861-169">Request</span></span>

<span data-ttu-id="ad861-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ad861-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="ad861-171">响应</span><span class="sxs-lookup"><span data-stu-id="ad861-171">Response</span></span>

<span data-ttu-id="ad861-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ad861-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="ad861-173">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="ad861-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="ad861-174">JSON</span><span class="sxs-lookup"><span data-stu-id="ad861-174">JSON</span></span>

<span data-ttu-id="ad861-175">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="ad861-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="ad861-176">请求</span><span class="sxs-lookup"><span data-stu-id="ad861-176">Request</span></span>

<span data-ttu-id="ad861-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ad861-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="ad861-178">响应</span><span class="sxs-lookup"><span data-stu-id="ad861-178">Response</span></span>

<span data-ttu-id="ad861-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ad861-179">The following is an example of the response.</span></span>

> <span data-ttu-id="ad861-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ad861-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
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


