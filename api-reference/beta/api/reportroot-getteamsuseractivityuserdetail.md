---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: 按用户获取有关 Microsoft Teams 用户活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: abf4b85d73a349a3fa3c4461c8d75311d2215e02
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896149"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="86a1b-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="86a1b-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="86a1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86a1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86a1b-105">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="86a1b-105">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="86a1b-106">权限</span><span class="sxs-lookup"><span data-stu-id="86a1b-106">Permissions</span></span>

<span data-ttu-id="86a1b-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="86a1b-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="86a1b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a1b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86a1b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86a1b-109">Permission type</span></span>                        | <span data-ttu-id="86a1b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86a1b-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="86a1b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86a1b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="86a1b-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="86a1b-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="86a1b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86a1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86a1b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86a1b-114">Not supported.</span></span>                           |
| <span data-ttu-id="86a1b-115">应用</span><span class="sxs-lookup"><span data-stu-id="86a1b-115">Application</span></span>                            | <span data-ttu-id="86a1b-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="86a1b-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="86a1b-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="86a1b-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="86a1b-118">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="86a1b-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="86a1b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86a1b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="86a1b-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="86a1b-120">Function parameters</span></span>

<span data-ttu-id="86a1b-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="86a1b-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="86a1b-122">参数</span><span class="sxs-lookup"><span data-stu-id="86a1b-122">Parameter</span></span> | <span data-ttu-id="86a1b-123">类型</span><span class="sxs-lookup"><span data-stu-id="86a1b-123">Type</span></span>   | <span data-ttu-id="86a1b-124">说明</span><span class="sxs-lookup"><span data-stu-id="86a1b-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="86a1b-125">period</span><span class="sxs-lookup"><span data-stu-id="86a1b-125">period</span></span>    | <span data-ttu-id="86a1b-126">string</span><span class="sxs-lookup"><span data-stu-id="86a1b-126">string</span></span> | <span data-ttu-id="86a1b-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="86a1b-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="86a1b-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="86a1b-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="86a1b-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="86a1b-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="86a1b-130">date</span><span class="sxs-lookup"><span data-stu-id="86a1b-130">date</span></span>      | <span data-ttu-id="86a1b-131">Date</span><span class="sxs-lookup"><span data-stu-id="86a1b-131">Date</span></span>   | <span data-ttu-id="86a1b-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="86a1b-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="86a1b-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="86a1b-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="86a1b-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="86a1b-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="86a1b-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="86a1b-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="86a1b-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="86a1b-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="86a1b-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="86a1b-137">The default output type is text/csv.</span></span> <span data-ttu-id="86a1b-138">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="86a1b-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86a1b-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="86a1b-139">Request headers</span></span>

| <span data-ttu-id="86a1b-140">名称</span><span class="sxs-lookup"><span data-stu-id="86a1b-140">Name</span></span>          | <span data-ttu-id="86a1b-141">说明</span><span class="sxs-lookup"><span data-stu-id="86a1b-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="86a1b-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="86a1b-142">Authorization</span></span> | <span data-ttu-id="86a1b-143">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="86a1b-143">Bearer {token}.</span></span> <span data-ttu-id="86a1b-144">Required.</span><span class="sxs-lookup"><span data-stu-id="86a1b-144">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="86a1b-145">响应</span><span class="sxs-lookup"><span data-stu-id="86a1b-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="86a1b-146">CSV</span><span class="sxs-lookup"><span data-stu-id="86a1b-146">CSV</span></span>

<span data-ttu-id="86a1b-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="86a1b-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="86a1b-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="86a1b-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="86a1b-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="86a1b-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="86a1b-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="86a1b-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="86a1b-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="86a1b-151">Report Refresh Date</span></span>
- <span data-ttu-id="86a1b-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="86a1b-152">User Principal Name</span></span>
- <span data-ttu-id="86a1b-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="86a1b-153">Last Activity Date</span></span>
- <span data-ttu-id="86a1b-154">已删除</span><span class="sxs-lookup"><span data-stu-id="86a1b-154">Is Deleted</span></span>
- <span data-ttu-id="86a1b-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="86a1b-155">Deleted Date</span></span>
- <span data-ttu-id="86a1b-156">分配的产品</span><span class="sxs-lookup"><span data-stu-id="86a1b-156">Assigned Products</span></span>
- <span data-ttu-id="86a1b-157">团队聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="86a1b-157">Team Chat Message Count</span></span>
- <span data-ttu-id="86a1b-158">专用聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="86a1b-158">Private Chat Message Count</span></span>
- <span data-ttu-id="86a1b-159">呼叫计数</span><span class="sxs-lookup"><span data-stu-id="86a1b-159">Call Count</span></span>
- <span data-ttu-id="86a1b-160">会议计数</span><span class="sxs-lookup"><span data-stu-id="86a1b-160">Meeting Count</span></span>
- <span data-ttu-id="86a1b-161">包含其他操作</span><span class="sxs-lookup"><span data-stu-id="86a1b-161">Has Other Action</span></span>
- <span data-ttu-id="86a1b-162">报表周期</span><span class="sxs-lookup"><span data-stu-id="86a1b-162">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="86a1b-163">JSON</span><span class="sxs-lookup"><span data-stu-id="86a1b-163">JSON</span></span>

<span data-ttu-id="86a1b-164">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="86a1b-164">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="86a1b-165">此请求的默认页面大小为2000个项目。</span><span class="sxs-lookup"><span data-stu-id="86a1b-165">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="86a1b-166">示例</span><span class="sxs-lookup"><span data-stu-id="86a1b-166">Example</span></span>

### <a name="csv"></a><span data-ttu-id="86a1b-167">CSV</span><span class="sxs-lookup"><span data-stu-id="86a1b-167">CSV</span></span>

<span data-ttu-id="86a1b-168">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="86a1b-168">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="86a1b-169">请求</span><span class="sxs-lookup"><span data-stu-id="86a1b-169">Request</span></span>

<span data-ttu-id="86a1b-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="86a1b-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="86a1b-171">响应</span><span class="sxs-lookup"><span data-stu-id="86a1b-171">Response</span></span>

<span data-ttu-id="86a1b-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86a1b-172">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="86a1b-173">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="86a1b-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```

### <a name="json"></a><span data-ttu-id="86a1b-174">JSON</span><span class="sxs-lookup"><span data-stu-id="86a1b-174">JSON</span></span>

<span data-ttu-id="86a1b-175">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="86a1b-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="86a1b-176">请求</span><span class="sxs-lookup"><span data-stu-id="86a1b-176">Request</span></span>

<span data-ttu-id="86a1b-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="86a1b-177">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="86a1b-178">响应</span><span class="sxs-lookup"><span data-stu-id="86a1b-178">Response</span></span>

<span data-ttu-id="86a1b-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86a1b-179">The following is an example of the response.</span></span>

> <span data-ttu-id="86a1b-180">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="86a1b-180">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="86a1b-181">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="86a1b-181">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "Microsoft 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "hasOtherAction": true, 
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
