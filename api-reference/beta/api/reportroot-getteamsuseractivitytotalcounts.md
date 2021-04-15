---
title: reportRoot： getTeamsUserActivityTotalCounts
description: 获取按活动类型的 Microsoft Teams 活动的数量。 活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。 这些活动由 Microsoft Teams 授权用户或非许可用户执行。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0c5acd7387638aba2fa3a992441982f5918be37f
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766907"
---
# <a name="reportroot-getteamsuseractivitytotalcounts"></a><span data-ttu-id="37832-105">reportRoot： getTeamsUserActivityTotalCounts</span><span class="sxs-lookup"><span data-stu-id="37832-105">reportRoot: getTeamsUserActivityTotalCounts</span></span>

<span data-ttu-id="37832-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37832-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37832-107">获取按活动类型的 Microsoft Teams 活动的数量。</span><span class="sxs-lookup"><span data-stu-id="37832-107">Get the number of Microsoft Teams activities by activity type.</span></span> <span data-ttu-id="37832-108">活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。</span><span class="sxs-lookup"><span data-stu-id="37832-108">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span> <span data-ttu-id="37832-109">这些活动由 Microsoft Teams 授权用户或非许可用户执行。</span><span class="sxs-lookup"><span data-stu-id="37832-109">The activities are performed by Microsoft Teams licensed or non-licensed users.</span></span>

## <a name="permissions"></a><span data-ttu-id="37832-110">权限</span><span class="sxs-lookup"><span data-stu-id="37832-110">Permissions</span></span>

<span data-ttu-id="37832-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37832-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37832-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="37832-113">Permission type</span></span>                        | <span data-ttu-id="37832-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37832-114">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="37832-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37832-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="37832-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="37832-116">Reports.Read.All</span></span>                         |
| <span data-ttu-id="37832-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37832-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37832-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="37832-118">Not supported.</span></span>                           |
| <span data-ttu-id="37832-119">应用</span><span class="sxs-lookup"><span data-stu-id="37832-119">Application</span></span>                            | <span data-ttu-id="37832-120">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="37832-120">Reports.Read.All</span></span>                         |

><span data-ttu-id="37832-121">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="37832-121">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="37832-122">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="37832-122">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="37832-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37832-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="37832-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="37832-124">Function parameters</span></span>

<span data-ttu-id="37832-125">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="37832-125">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="37832-126">参数</span><span class="sxs-lookup"><span data-stu-id="37832-126">Parameter</span></span> | <span data-ttu-id="37832-127">类型</span><span class="sxs-lookup"><span data-stu-id="37832-127">Type</span></span>   | <span data-ttu-id="37832-128">说明</span><span class="sxs-lookup"><span data-stu-id="37832-128">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="37832-129">period</span><span class="sxs-lookup"><span data-stu-id="37832-129">period</span></span>    | <span data-ttu-id="37832-130">string</span><span class="sxs-lookup"><span data-stu-id="37832-130">string</span></span> | <span data-ttu-id="37832-131">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="37832-131">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="37832-132">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="37832-132">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="37832-133">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="37832-133">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="37832-134">必需。</span><span class="sxs-lookup"><span data-stu-id="37832-134">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="37832-135">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="37832-135">Optional query parameters</span></span>

<span data-ttu-id="37832-136">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="37832-136">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="37832-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="37832-137">The default output type is text/csv.</span></span> <span data-ttu-id="37832-138">但是，如果要指定输出类型，可以使用设置为 text/csv 或 application/json 的 OData `$format` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="37832-138">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37832-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="37832-139">Request headers</span></span>

| <span data-ttu-id="37832-140">名称</span><span class="sxs-lookup"><span data-stu-id="37832-140">Name</span></span>          | <span data-ttu-id="37832-141">说明</span><span class="sxs-lookup"><span data-stu-id="37832-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="37832-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="37832-142">Authorization</span></span> | <span data-ttu-id="37832-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37832-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="37832-145">响应</span><span class="sxs-lookup"><span data-stu-id="37832-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="37832-146">CSV</span><span class="sxs-lookup"><span data-stu-id="37832-146">CSV</span></span>

<span data-ttu-id="37832-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="37832-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="37832-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="37832-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="37832-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="37832-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="37832-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="37832-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="37832-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="37832-151">Report Refresh Date</span></span>
- <span data-ttu-id="37832-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="37832-152">Report Date</span></span>
- <span data-ttu-id="37832-153">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="37832-153">Team Chat Messages</span></span>
- <span data-ttu-id="37832-154">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="37832-154">Private Chat Messages</span></span>
- <span data-ttu-id="37832-155">呼叫</span><span class="sxs-lookup"><span data-stu-id="37832-155">Calls</span></span>
- <span data-ttu-id="37832-156">会议</span><span class="sxs-lookup"><span data-stu-id="37832-156">Meetings</span></span>
- <span data-ttu-id="37832-157">报表周期</span><span class="sxs-lookup"><span data-stu-id="37832-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="37832-158">JSON</span><span class="sxs-lookup"><span data-stu-id="37832-158">JSON</span></span>

<span data-ttu-id="37832-159">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37832-159">If successful, this method returns a `200 OK` response code and a [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37832-160">示例</span><span class="sxs-lookup"><span data-stu-id="37832-160">Example</span></span>

### <a name="csv"></a><span data-ttu-id="37832-161">CSV</span><span class="sxs-lookup"><span data-stu-id="37832-161">CSV</span></span>

<span data-ttu-id="37832-162">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="37832-162">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="37832-163">请求</span><span class="sxs-lookup"><span data-stu-id="37832-163">Request</span></span>

<span data-ttu-id="37832-164">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="37832-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="37832-165">响应</span><span class="sxs-lookup"><span data-stu-id="37832-165">Response</span></span>

<span data-ttu-id="37832-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="37832-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
<span data-ttu-id="37832-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="37832-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="37832-168">JSON</span><span class="sxs-lookup"><span data-stu-id="37832-168">JSON</span></span>

<span data-ttu-id="37832-169">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="37832-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="37832-170">请求</span><span class="sxs-lookup"><span data-stu-id="37832-170">Request</span></span>

<span data-ttu-id="37832-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="37832-171">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="37832-172">响应</span><span class="sxs-lookup"><span data-stu-id="37832-172">Response</span></span>

<span data-ttu-id="37832-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="37832-173">The following is an example of the response.</span></span>

> <span data-ttu-id="37832-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="37832-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
