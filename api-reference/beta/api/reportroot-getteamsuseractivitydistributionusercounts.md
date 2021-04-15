---
title: reportRoot： getTeamsUserActivityDistributionUserCounts
description: 按活动类型获取选定时段内 Microsoft Teams 许可用户的数量。 活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 91a9f503ad2798f154d7415e93e7c4be28cd7c32
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766915"
---
# <a name="reportroot-getteamsuseractivitydistributionusercounts"></a><span data-ttu-id="1b7cd-104">reportRoot： getTeamsUserActivityDistributionUserCounts</span><span class="sxs-lookup"><span data-stu-id="1b7cd-104">reportRoot: getTeamsUserActivityDistributionUserCounts</span></span>

<span data-ttu-id="1b7cd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b7cd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b7cd-106">按活动类型获取选定时段内 Microsoft Teams 许可用户的数量。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-106">Get the number of Microsoft Teams licensed users by activity type over the selected period.</span></span> <span data-ttu-id="1b7cd-107">活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-107">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b7cd-108">权限</span><span class="sxs-lookup"><span data-stu-id="1b7cd-108">Permissions</span></span>

<span data-ttu-id="1b7cd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b7cd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b7cd-111">Permission type</span></span>                        | <span data-ttu-id="1b7cd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b7cd-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1b7cd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b7cd-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b7cd-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b7cd-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1b7cd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b7cd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b7cd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-116">Not supported.</span></span>                           |
| <span data-ttu-id="1b7cd-117">应用</span><span class="sxs-lookup"><span data-stu-id="1b7cd-117">Application</span></span>                            | <span data-ttu-id="1b7cd-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b7cd-118">Reports.Read.All</span></span>                         |

> <span data-ttu-id="1b7cd-119">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="1b7cd-120">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="1b7cd-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b7cd-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityDistributionUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="1b7cd-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="1b7cd-122">Function parameters</span></span>

<span data-ttu-id="1b7cd-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1b7cd-124">参数</span><span class="sxs-lookup"><span data-stu-id="1b7cd-124">Parameter</span></span> | <span data-ttu-id="1b7cd-125">类型</span><span class="sxs-lookup"><span data-stu-id="1b7cd-125">Type</span></span>   | <span data-ttu-id="1b7cd-126">说明</span><span class="sxs-lookup"><span data-stu-id="1b7cd-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1b7cd-127">period</span><span class="sxs-lookup"><span data-stu-id="1b7cd-127">period</span></span>    | <span data-ttu-id="1b7cd-128">string</span><span class="sxs-lookup"><span data-stu-id="1b7cd-128">string</span></span> | <span data-ttu-id="1b7cd-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1b7cd-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1b7cd-131">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1b7cd-132">必需。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-132">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="1b7cd-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1b7cd-133">Optional query parameters</span></span>

<span data-ttu-id="1b7cd-134">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1b7cd-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-135">The default output type is text/csv.</span></span> <span data-ttu-id="1b7cd-136">但是，如果要指定输出类型，可以使用设置为 text/csv 或 application/json 的 OData `$format` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-136">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b7cd-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b7cd-137">Request headers</span></span>

| <span data-ttu-id="1b7cd-138">名称</span><span class="sxs-lookup"><span data-stu-id="1b7cd-138">Name</span></span>          | <span data-ttu-id="1b7cd-139">说明</span><span class="sxs-lookup"><span data-stu-id="1b7cd-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1b7cd-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b7cd-140">Authorization</span></span> | <span data-ttu-id="1b7cd-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1b7cd-143">响应</span><span class="sxs-lookup"><span data-stu-id="1b7cd-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1b7cd-144">CSV</span><span class="sxs-lookup"><span data-stu-id="1b7cd-144">CSV</span></span>

<span data-ttu-id="1b7cd-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1b7cd-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1b7cd-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1b7cd-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1b7cd-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="1b7cd-149">Report Refresh Date</span></span>
- <span data-ttu-id="1b7cd-150">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="1b7cd-150">Team Chat Messages</span></span>
- <span data-ttu-id="1b7cd-151">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="1b7cd-151">Private Chat Messages</span></span>
- <span data-ttu-id="1b7cd-152">呼叫</span><span class="sxs-lookup"><span data-stu-id="1b7cd-152">Calls</span></span>
- <span data-ttu-id="1b7cd-153">会议</span><span class="sxs-lookup"><span data-stu-id="1b7cd-153">Meetings</span></span>
- <span data-ttu-id="1b7cd-154">报表周期</span><span class="sxs-lookup"><span data-stu-id="1b7cd-154">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1b7cd-155">JSON</span><span class="sxs-lookup"><span data-stu-id="1b7cd-155">JSON</span></span>

<span data-ttu-id="1b7cd-156">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-156">If successful, this method returns a `200 OK` response code and a [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b7cd-157">示例</span><span class="sxs-lookup"><span data-stu-id="1b7cd-157">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1b7cd-158">CSV</span><span class="sxs-lookup"><span data-stu-id="1b7cd-158">CSV</span></span>

<span data-ttu-id="1b7cd-159">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-159">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1b7cd-160">请求</span><span class="sxs-lookup"><span data-stu-id="1b7cd-160">Request</span></span>

<span data-ttu-id="1b7cd-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-161">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributionusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="1b7cd-162">响应</span><span class="sxs-lookup"><span data-stu-id="1b7cd-162">Response</span></span>

<span data-ttu-id="1b7cd-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1b7cd-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Report Period
```

### <a name="json"></a><span data-ttu-id="1b7cd-165">JSON</span><span class="sxs-lookup"><span data-stu-id="1b7cd-165">JSON</span></span>

<span data-ttu-id="1b7cd-166">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1b7cd-167">请求</span><span class="sxs-lookup"><span data-stu-id="1b7cd-167">Request</span></span>

<span data-ttu-id="1b7cd-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitydistributionusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityDistributionUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="1b7cd-169">响应</span><span class="sxs-lookup"><span data-stu-id="1b7cd-169">Response</span></span>

<span data-ttu-id="1b7cd-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-170">The following is an example of the response.</span></span>

> <span data-ttu-id="1b7cd-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1b7cd-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsuseractivitydistributionusercounts)", 
  "value": [
    {
      "reportRefreshDate": "2020-09-01", 
      "teamChatMessages": 0, 
      "privateChatMessages": 0, 
      "calls": 0, 
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


