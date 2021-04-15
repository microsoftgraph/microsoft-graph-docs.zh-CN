---
title: reportRoot： getTeamsUserActivityTotalUserCounts
description: 按活动类型获取 Microsoft Teams 许可或非许可用户的数量。 活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9c62a7bf316f8b11b908f30eb3db1865b7a4f1df
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766919"
---
# <a name="reportroot-getteamsuseractivitytotalusercounts"></a><span data-ttu-id="2688c-104">reportRoot： getTeamsUserActivityTotalUserCounts</span><span class="sxs-lookup"><span data-stu-id="2688c-104">reportRoot: getTeamsUserActivityTotalUserCounts</span></span>

<span data-ttu-id="2688c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2688c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2688c-106">按活动类型获取 Microsoft Teams 许可或非许可用户的数量。</span><span class="sxs-lookup"><span data-stu-id="2688c-106">Get the number of Microsoft Teams licensed or non-licensed users by activity type.</span></span> <span data-ttu-id="2688c-107">活动类型包括团队聊天消息、私人聊天消息、通话和会议的数量。</span><span class="sxs-lookup"><span data-stu-id="2688c-107">The activity types are number of teams chat messages, private chat messages, calls, and meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="2688c-108">权限</span><span class="sxs-lookup"><span data-stu-id="2688c-108">Permissions</span></span>

<span data-ttu-id="2688c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2688c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2688c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2688c-111">Permission type</span></span>                        | <span data-ttu-id="2688c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2688c-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2688c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2688c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2688c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2688c-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2688c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2688c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2688c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2688c-116">Not supported.</span></span>                           |
| <span data-ttu-id="2688c-117">应用</span><span class="sxs-lookup"><span data-stu-id="2688c-117">Application</span></span>                            | <span data-ttu-id="2688c-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2688c-118">Reports.Read.All</span></span>                         |

> <span data-ttu-id="2688c-119">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="2688c-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="2688c-120">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="2688c-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="2688c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2688c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityTotalUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="2688c-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="2688c-122">Function parameters</span></span>

<span data-ttu-id="2688c-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="2688c-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2688c-124">参数</span><span class="sxs-lookup"><span data-stu-id="2688c-124">Parameter</span></span> | <span data-ttu-id="2688c-125">类型</span><span class="sxs-lookup"><span data-stu-id="2688c-125">Type</span></span>   | <span data-ttu-id="2688c-126">说明</span><span class="sxs-lookup"><span data-stu-id="2688c-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2688c-127">period</span><span class="sxs-lookup"><span data-stu-id="2688c-127">period</span></span>    | <span data-ttu-id="2688c-128">string</span><span class="sxs-lookup"><span data-stu-id="2688c-128">string</span></span> | <span data-ttu-id="2688c-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2688c-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2688c-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="2688c-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2688c-131">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2688c-131">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2688c-132">必需。</span><span class="sxs-lookup"><span data-stu-id="2688c-132">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="2688c-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2688c-133">Optional query parameters</span></span>

<span data-ttu-id="2688c-134">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2688c-134">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="2688c-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="2688c-135">The default output type is text/csv.</span></span> <span data-ttu-id="2688c-136">但是，如果要指定输出类型，可以使用设置为 text/csv 或 application/json 的 OData `$format` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="2688c-136">However, if you want to specify the output type, you can use the OData `$format` query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2688c-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="2688c-137">Request headers</span></span>

| <span data-ttu-id="2688c-138">名称</span><span class="sxs-lookup"><span data-stu-id="2688c-138">Name</span></span>          | <span data-ttu-id="2688c-139">说明</span><span class="sxs-lookup"><span data-stu-id="2688c-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="2688c-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="2688c-140">Authorization</span></span> | <span data-ttu-id="2688c-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2688c-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2688c-143">响应</span><span class="sxs-lookup"><span data-stu-id="2688c-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="2688c-144">CSV</span><span class="sxs-lookup"><span data-stu-id="2688c-144">CSV</span></span>

<span data-ttu-id="2688c-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2688c-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2688c-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2688c-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2688c-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="2688c-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2688c-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="2688c-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2688c-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2688c-149">Report Refresh Date</span></span>
- <span data-ttu-id="2688c-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="2688c-150">Report Date</span></span>
- <span data-ttu-id="2688c-151">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="2688c-151">Team Chat Messages</span></span>
- <span data-ttu-id="2688c-152">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="2688c-152">Private Chat Messages</span></span>
- <span data-ttu-id="2688c-153">呼叫</span><span class="sxs-lookup"><span data-stu-id="2688c-153">Calls</span></span>
- <span data-ttu-id="2688c-154">会议</span><span class="sxs-lookup"><span data-stu-id="2688c-154">Meetings</span></span>
- <span data-ttu-id="2688c-155">其他操作</span><span class="sxs-lookup"><span data-stu-id="2688c-155">Other Actions</span></span>
- <span data-ttu-id="2688c-156">报表周期</span><span class="sxs-lookup"><span data-stu-id="2688c-156">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="2688c-157">JSON</span><span class="sxs-lookup"><span data-stu-id="2688c-157">JSON</span></span>

<span data-ttu-id="2688c-158">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2688c-158">If successful, this method returns a `200 OK` response code and a [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2688c-159">示例</span><span class="sxs-lookup"><span data-stu-id="2688c-159">Example</span></span>

### <a name="csv"></a><span data-ttu-id="2688c-160">CSV</span><span class="sxs-lookup"><span data-stu-id="2688c-160">CSV</span></span>

<span data-ttu-id="2688c-161">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="2688c-161">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="2688c-162">请求</span><span class="sxs-lookup"><span data-stu-id="2688c-162">Request</span></span>

<span data-ttu-id="2688c-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2688c-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="2688c-164">响应</span><span class="sxs-lookup"><span data-stu-id="2688c-164">Response</span></span>

<span data-ttu-id="2688c-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2688c-165">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="2688c-166">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2688c-166">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Team Chat Messages,Private Chat Messages,Calls,Meetings,Other Actions,Report Period
```

### <a name="json"></a><span data-ttu-id="2688c-167">JSON</span><span class="sxs-lookup"><span data-stu-id="2688c-167">JSON</span></span>

<span data-ttu-id="2688c-168">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="2688c-168">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="2688c-169">请求</span><span class="sxs-lookup"><span data-stu-id="2688c-169">Request</span></span>

<span data-ttu-id="2688c-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2688c-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivitytotalusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityTotalUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="2688c-171">响应</span><span class="sxs-lookup"><span data-stu-id="2688c-171">Response</span></span>

<span data-ttu-id="2688c-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2688c-172">The following is an example of the response.</span></span>

> <span data-ttu-id="2688c-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2688c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "reportDate": "2017-09-01", 
      "teamChatMessages": 30, 
      "privateChatMessages": 21, 
      "calls": 6, 
      "meetings": 2, 
      "otherActions": 17, 
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
