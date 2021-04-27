---
title: 'reportRoot: getTeamsUserActivityCounts'
description: 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。 活动由许可Microsoft Teams执行。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: be6fd27c9e4b99e8d8311bf9f60e2ee057ac4ce2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049042"
---
# <a name="reportroot-getteamsuseractivitycounts"></a><span data-ttu-id="e6785-105">reportRoot: getTeamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="e6785-105">reportRoot: getTeamsUserActivityCounts</span></span>

<span data-ttu-id="e6785-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6785-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6785-107">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="e6785-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="e6785-108">活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。</span><span class="sxs-lookup"><span data-stu-id="e6785-108">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span> <span data-ttu-id="e6785-109">活动由许可Microsoft Teams执行。</span><span class="sxs-lookup"><span data-stu-id="e6785-109">The activities are performed by Microsoft Teams licensed users.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6785-110">权限</span><span class="sxs-lookup"><span data-stu-id="e6785-110">Permissions</span></span>

<span data-ttu-id="e6785-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6785-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6785-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6785-113">Permission type</span></span>                        | <span data-ttu-id="e6785-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6785-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e6785-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6785-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6785-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6785-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e6785-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6785-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6785-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6785-118">Not supported.</span></span>                           |
| <span data-ttu-id="e6785-119">应用</span><span class="sxs-lookup"><span data-stu-id="e6785-119">Application</span></span>                            | <span data-ttu-id="e6785-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6785-120">Reports.Read.All</span></span>                         |

<span data-ttu-id="e6785-121">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e6785-121">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="e6785-122">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="e6785-122">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="e6785-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6785-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="e6785-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="e6785-124">Function parameters</span></span>

<span data-ttu-id="e6785-125">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="e6785-125">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e6785-126">参数</span><span class="sxs-lookup"><span data-stu-id="e6785-126">Parameter</span></span> | <span data-ttu-id="e6785-127">类型</span><span class="sxs-lookup"><span data-stu-id="e6785-127">Type</span></span>   | <span data-ttu-id="e6785-128">说明</span><span class="sxs-lookup"><span data-stu-id="e6785-128">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e6785-129">period</span><span class="sxs-lookup"><span data-stu-id="e6785-129">period</span></span>    | <span data-ttu-id="e6785-130">string</span><span class="sxs-lookup"><span data-stu-id="e6785-130">string</span></span> | <span data-ttu-id="e6785-131">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e6785-131">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e6785-132">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e6785-132">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e6785-133">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e6785-133">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e6785-134">必需。</span><span class="sxs-lookup"><span data-stu-id="e6785-134">Required.</span></span> |

<span data-ttu-id="e6785-135">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e6785-135">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e6785-136">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="e6785-136">The default output type is text/csv.</span></span> <span data-ttu-id="e6785-137">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="e6785-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6785-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6785-138">Request headers</span></span>

| <span data-ttu-id="e6785-139">名称</span><span class="sxs-lookup"><span data-stu-id="e6785-139">Name</span></span>          | <span data-ttu-id="e6785-140">说明</span><span class="sxs-lookup"><span data-stu-id="e6785-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e6785-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6785-141">Authorization</span></span> | <span data-ttu-id="e6785-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6785-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e6785-144">响应</span><span class="sxs-lookup"><span data-stu-id="e6785-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e6785-145">CSV</span><span class="sxs-lookup"><span data-stu-id="e6785-145">CSV</span></span>

<span data-ttu-id="e6785-146">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e6785-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e6785-147">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e6785-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e6785-148">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e6785-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e6785-149">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e6785-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e6785-150">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e6785-150">Report Refresh Date</span></span>
- <span data-ttu-id="e6785-151">报表日期</span><span class="sxs-lookup"><span data-stu-id="e6785-151">Report Date</span></span>
- <span data-ttu-id="e6785-152">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="e6785-152">Team Chat Messages</span></span>
- <span data-ttu-id="e6785-153">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="e6785-153">Private Chat Messages</span></span>
- <span data-ttu-id="e6785-154">呼叫</span><span class="sxs-lookup"><span data-stu-id="e6785-154">Calls</span></span>
- <span data-ttu-id="e6785-155">会议</span><span class="sxs-lookup"><span data-stu-id="e6785-155">Meetings</span></span>
- <span data-ttu-id="e6785-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="e6785-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e6785-157">JSON</span><span class="sxs-lookup"><span data-stu-id="e6785-157">JSON</span></span>

<span data-ttu-id="e6785-158">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="e6785-158">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityCounts](../resources/teamsuseractivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6785-159">示例</span><span class="sxs-lookup"><span data-stu-id="e6785-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e6785-160">CSV</span><span class="sxs-lookup"><span data-stu-id="e6785-160">CSV</span></span>

<span data-ttu-id="e6785-161">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="e6785-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e6785-162">请求</span><span class="sxs-lookup"><span data-stu-id="e6785-162">Request</span></span>

<span data-ttu-id="e6785-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e6785-163">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="e6785-164">响应</span><span class="sxs-lookup"><span data-stu-id="e6785-164">Response</span></span>

<span data-ttu-id="e6785-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e6785-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="e6785-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e6785-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="e6785-167">JSON</span><span class="sxs-lookup"><span data-stu-id="e6785-167">JSON</span></span>

<span data-ttu-id="e6785-168">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="e6785-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e6785-169">请求</span><span class="sxs-lookup"><span data-stu-id="e6785-169">Request</span></span>

<span data-ttu-id="e6785-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e6785-170">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="e6785-171">响应</span><span class="sxs-lookup"><span data-stu-id="e6785-171">Response</span></span>

<span data-ttu-id="e6785-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e6785-172">The following is an example of the response.</span></span>

> <span data-ttu-id="e6785-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e6785-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 26, 
      "privateChatMessages": 17, 
      "calls": 4, 
      "meetings": 0, 
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


