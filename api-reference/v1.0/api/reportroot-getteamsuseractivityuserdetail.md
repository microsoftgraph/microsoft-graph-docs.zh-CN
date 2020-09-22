---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: 按用户获取有关 Microsoft Teams 用户活动的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7932844945de2255fb07adf16cdd943c65421c7f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038352"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="97100-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="97100-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="97100-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97100-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97100-105">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="97100-105">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="97100-106">权限</span><span class="sxs-lookup"><span data-stu-id="97100-106">Permissions</span></span>

<span data-ttu-id="97100-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97100-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97100-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97100-109">Permission type</span></span>                        | <span data-ttu-id="97100-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97100-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="97100-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97100-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="97100-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="97100-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="97100-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97100-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97100-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="97100-114">Not supported.</span></span>                           |
| <span data-ttu-id="97100-115">应用</span><span class="sxs-lookup"><span data-stu-id="97100-115">Application</span></span>                            | <span data-ttu-id="97100-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="97100-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="97100-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="97100-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="97100-118">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="97100-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="97100-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97100-119">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="97100-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="97100-120">Function parameters</span></span>

<span data-ttu-id="97100-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="97100-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="97100-122">参数</span><span class="sxs-lookup"><span data-stu-id="97100-122">Parameter</span></span> | <span data-ttu-id="97100-123">类型</span><span class="sxs-lookup"><span data-stu-id="97100-123">Type</span></span>   | <span data-ttu-id="97100-124">说明</span><span class="sxs-lookup"><span data-stu-id="97100-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="97100-125">period</span><span class="sxs-lookup"><span data-stu-id="97100-125">period</span></span>    | <span data-ttu-id="97100-126">string</span><span class="sxs-lookup"><span data-stu-id="97100-126">string</span></span> | <span data-ttu-id="97100-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="97100-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="97100-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="97100-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="97100-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="97100-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="97100-130">date</span><span class="sxs-lookup"><span data-stu-id="97100-130">date</span></span>      | <span data-ttu-id="97100-131">Date</span><span class="sxs-lookup"><span data-stu-id="97100-131">Date</span></span>   | <span data-ttu-id="97100-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="97100-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="97100-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="97100-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="97100-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="97100-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="97100-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="97100-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97100-136">请求头</span><span class="sxs-lookup"><span data-stu-id="97100-136">Request headers</span></span>

| <span data-ttu-id="97100-137">名称</span><span class="sxs-lookup"><span data-stu-id="97100-137">Name</span></span>          | <span data-ttu-id="97100-138">说明</span><span class="sxs-lookup"><span data-stu-id="97100-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="97100-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="97100-139">Authorization</span></span> | <span data-ttu-id="97100-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97100-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="97100-142">响应</span><span class="sxs-lookup"><span data-stu-id="97100-142">Response</span></span>

<span data-ttu-id="97100-143">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="97100-143">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="97100-144">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="97100-144">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="97100-145">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="97100-145">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="97100-146">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="97100-146">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="97100-147">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="97100-147">Report Refresh Date</span></span>
- <span data-ttu-id="97100-148">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="97100-148">User Principal Name</span></span>
- <span data-ttu-id="97100-149">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="97100-149">Last Activity Date</span></span>
- <span data-ttu-id="97100-150">已删除</span><span class="sxs-lookup"><span data-stu-id="97100-150">Is Deleted</span></span>
- <span data-ttu-id="97100-151">删除日期</span><span class="sxs-lookup"><span data-stu-id="97100-151">Deleted Date</span></span>
- <span data-ttu-id="97100-152">分配的产品</span><span class="sxs-lookup"><span data-stu-id="97100-152">Assigned Products</span></span>
- <span data-ttu-id="97100-153">团队聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="97100-153">Team Chat Message Count</span></span>
- <span data-ttu-id="97100-154">专用聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="97100-154">Private Chat Message Count</span></span>
- <span data-ttu-id="97100-155">呼叫计数</span><span class="sxs-lookup"><span data-stu-id="97100-155">Call Count</span></span>
- <span data-ttu-id="97100-156">会议计数</span><span class="sxs-lookup"><span data-stu-id="97100-156">Meeting Count</span></span>
- <span data-ttu-id="97100-157">包含其他操作</span><span class="sxs-lookup"><span data-stu-id="97100-157">Has Other Action</span></span>
- <span data-ttu-id="97100-158">报表周期</span><span class="sxs-lookup"><span data-stu-id="97100-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="97100-159">示例</span><span class="sxs-lookup"><span data-stu-id="97100-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="97100-160">请求</span><span class="sxs-lookup"><span data-stu-id="97100-160">Request</span></span>

<span data-ttu-id="97100-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="97100-161">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="97100-162">响应</span><span class="sxs-lookup"><span data-stu-id="97100-162">Response</span></span>

<span data-ttu-id="97100-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="97100-163">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.report"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="97100-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="97100-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
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

