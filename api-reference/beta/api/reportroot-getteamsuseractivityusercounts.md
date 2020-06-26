---
title: 'reportRoot: getTeamsUserActivityUserCounts'
description: 按活动类型获取 Microsoft Teams 用户的数量。 活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8c895b60774b4c8d0496e9702c8f0202f7b43acb
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896145"
---
# <a name="reportroot-getteamsuseractivityusercounts"></a><span data-ttu-id="7519a-104">reportRoot: getTeamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7519a-104">reportRoot: getTeamsUserActivityUserCounts</span></span>

<span data-ttu-id="7519a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7519a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7519a-106">按活动类型获取 Microsoft Teams 用户的数量。</span><span class="sxs-lookup"><span data-stu-id="7519a-106">Get the number of Microsoft Teams users by activity type.</span></span> <span data-ttu-id="7519a-107">活动类型是许多团队聊天消息、专用聊天消息、呼叫或会议。</span><span class="sxs-lookup"><span data-stu-id="7519a-107">The activity types are number of teams chat messages, private chat messages, calls, or meetings.</span></span>

## <a name="permissions"></a><span data-ttu-id="7519a-108">权限</span><span class="sxs-lookup"><span data-stu-id="7519a-108">Permissions</span></span>

<span data-ttu-id="7519a-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="7519a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="7519a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7519a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7519a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7519a-111">Permission type</span></span>                        | <span data-ttu-id="7519a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7519a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7519a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7519a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7519a-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7519a-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7519a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7519a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7519a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7519a-116">Not supported.</span></span>                           |
| <span data-ttu-id="7519a-117">应用</span><span class="sxs-lookup"><span data-stu-id="7519a-117">Application</span></span>                            | <span data-ttu-id="7519a-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7519a-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="7519a-119">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="7519a-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="7519a-120">有关更多详细信息，请参阅[授权 For api 以读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="7519a-120">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="7519a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7519a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserCounts(period='D7')
```

## <a name="function-parameters"></a><span data-ttu-id="7519a-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="7519a-122">Function parameters</span></span>

<span data-ttu-id="7519a-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7519a-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7519a-124">参数</span><span class="sxs-lookup"><span data-stu-id="7519a-124">Parameter</span></span> | <span data-ttu-id="7519a-125">类型</span><span class="sxs-lookup"><span data-stu-id="7519a-125">Type</span></span>   | <span data-ttu-id="7519a-126">说明</span><span class="sxs-lookup"><span data-stu-id="7519a-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7519a-127">period</span><span class="sxs-lookup"><span data-stu-id="7519a-127">period</span></span>    | <span data-ttu-id="7519a-128">string</span><span class="sxs-lookup"><span data-stu-id="7519a-128">string</span></span> | <span data-ttu-id="7519a-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7519a-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7519a-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7519a-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7519a-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7519a-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7519a-132">必需。</span><span class="sxs-lookup"><span data-stu-id="7519a-132">Required.</span></span> |

<span data-ttu-id="7519a-133">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7519a-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7519a-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="7519a-134">The default output type is text/csv.</span></span> <span data-ttu-id="7519a-135">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="7519a-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7519a-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="7519a-136">Request headers</span></span>

| <span data-ttu-id="7519a-137">名称</span><span class="sxs-lookup"><span data-stu-id="7519a-137">Name</span></span>          | <span data-ttu-id="7519a-138">说明</span><span class="sxs-lookup"><span data-stu-id="7519a-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7519a-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="7519a-139">Authorization</span></span> | <span data-ttu-id="7519a-140">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="7519a-140">Bearer {token}.</span></span> <span data-ttu-id="7519a-141">Required.</span><span class="sxs-lookup"><span data-stu-id="7519a-141">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7519a-142">响应</span><span class="sxs-lookup"><span data-stu-id="7519a-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7519a-143">CSV</span><span class="sxs-lookup"><span data-stu-id="7519a-143">CSV</span></span>

<span data-ttu-id="7519a-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7519a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7519a-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7519a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7519a-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7519a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7519a-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7519a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7519a-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7519a-148">Report Refresh Date</span></span>
- <span data-ttu-id="7519a-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="7519a-149">Report Date</span></span>
- <span data-ttu-id="7519a-150">团队聊天消息</span><span class="sxs-lookup"><span data-stu-id="7519a-150">Team Chat Messages</span></span>
- <span data-ttu-id="7519a-151">专用聊天消息</span><span class="sxs-lookup"><span data-stu-id="7519a-151">Private Chat Messages</span></span>
- <span data-ttu-id="7519a-152">呼叫</span><span class="sxs-lookup"><span data-stu-id="7519a-152">Calls</span></span>
- <span data-ttu-id="7519a-153">会议</span><span class="sxs-lookup"><span data-stu-id="7519a-153">Meetings</span></span>
- <span data-ttu-id="7519a-154">其他操作</span><span class="sxs-lookup"><span data-stu-id="7519a-154">Other Actions</span></span>
- <span data-ttu-id="7519a-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="7519a-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7519a-156">JSON</span><span class="sxs-lookup"><span data-stu-id="7519a-156">JSON</span></span>

<span data-ttu-id="7519a-157">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和**[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="7519a-157">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7519a-158">示例</span><span class="sxs-lookup"><span data-stu-id="7519a-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7519a-159">CSV</span><span class="sxs-lookup"><span data-stu-id="7519a-159">CSV</span></span>

<span data-ttu-id="7519a-160">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="7519a-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7519a-161">请求</span><span class="sxs-lookup"><span data-stu-id="7519a-161">Request</span></span>

<span data-ttu-id="7519a-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7519a-162">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="7519a-163">响应</span><span class="sxs-lookup"><span data-stu-id="7519a-163">Response</span></span>

<span data-ttu-id="7519a-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7519a-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="7519a-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7519a-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="7519a-166">JSON</span><span class="sxs-lookup"><span data-stu-id="7519a-166">JSON</span></span>

<span data-ttu-id="7519a-167">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="7519a-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7519a-168">请求</span><span class="sxs-lookup"><span data-stu-id="7519a-168">Request</span></span>

<span data-ttu-id="7519a-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7519a-169">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserCounts(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="7519a-170">响应</span><span class="sxs-lookup"><span data-stu-id="7519a-170">Response</span></span>

<span data-ttu-id="7519a-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7519a-171">The following is an example of the response.</span></span>

> <span data-ttu-id="7519a-172">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="7519a-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7519a-173">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="7519a-173">All the properties will be returned from an actual call.</span></span>

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
