---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: 按用户获取有关 Microsoft Teams 用户活动的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e432abf6e1b6d8cc0906709319543a1c7905771d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603551"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="66458-103">reportRoot：getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="66458-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="66458-104">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="66458-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="66458-105">权限</span><span class="sxs-lookup"><span data-stu-id="66458-105">Permissions</span></span>

<span data-ttu-id="66458-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66458-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="66458-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="66458-108">Permission type</span></span>                        | <span data-ttu-id="66458-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66458-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="66458-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66458-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="66458-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="66458-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="66458-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66458-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66458-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="66458-113">Not supported.</span></span>                           |
| <span data-ttu-id="66458-114">应用</span><span class="sxs-lookup"><span data-stu-id="66458-114">Application</span></span>                            | <span data-ttu-id="66458-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="66458-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="66458-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66458-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="66458-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="66458-117">Function parameters</span></span>

<span data-ttu-id="66458-118">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="66458-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="66458-119">参数</span><span class="sxs-lookup"><span data-stu-id="66458-119">Parameter</span></span> | <span data-ttu-id="66458-120">类型</span><span class="sxs-lookup"><span data-stu-id="66458-120">Type</span></span>   | <span data-ttu-id="66458-121">说明</span><span class="sxs-lookup"><span data-stu-id="66458-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="66458-122">period</span><span class="sxs-lookup"><span data-stu-id="66458-122">period</span></span>    | <span data-ttu-id="66458-123">string</span><span class="sxs-lookup"><span data-stu-id="66458-123">string</span></span> | <span data-ttu-id="66458-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="66458-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="66458-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="66458-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="66458-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="66458-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="66458-127">date</span><span class="sxs-lookup"><span data-stu-id="66458-127">date</span></span>      | <span data-ttu-id="66458-128">Date</span><span class="sxs-lookup"><span data-stu-id="66458-128">Date</span></span>   | <span data-ttu-id="66458-129">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="66458-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="66458-130">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="66458-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="66458-131">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="66458-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="66458-132">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="66458-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66458-133">请求头</span><span class="sxs-lookup"><span data-stu-id="66458-133">Request headers</span></span>

| <span data-ttu-id="66458-134">名称</span><span class="sxs-lookup"><span data-stu-id="66458-134">Name</span></span>          | <span data-ttu-id="66458-135">说明</span><span class="sxs-lookup"><span data-stu-id="66458-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="66458-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="66458-136">Authorization</span></span> | <span data-ttu-id="66458-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66458-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="66458-139">响应</span><span class="sxs-lookup"><span data-stu-id="66458-139">Response</span></span>

<span data-ttu-id="66458-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="66458-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="66458-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="66458-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="66458-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="66458-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="66458-143">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="66458-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="66458-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="66458-144">Report Refresh Date</span></span>
- <span data-ttu-id="66458-145">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="66458-145">User Principal Name</span></span>
- <span data-ttu-id="66458-146">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="66458-146">Last Activity Date</span></span>
- <span data-ttu-id="66458-147">已删除</span><span class="sxs-lookup"><span data-stu-id="66458-147">Is Deleted</span></span>
- <span data-ttu-id="66458-148">删除日期</span><span class="sxs-lookup"><span data-stu-id="66458-148">Deleted Date</span></span>
- <span data-ttu-id="66458-149">分配的产品</span><span class="sxs-lookup"><span data-stu-id="66458-149">Assigned Products</span></span>
- <span data-ttu-id="66458-150">团队聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="66458-150">Team Chat Message Count</span></span>
- <span data-ttu-id="66458-151">专用聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="66458-151">Private Chat Message Count</span></span>
- <span data-ttu-id="66458-152">呼叫计数</span><span class="sxs-lookup"><span data-stu-id="66458-152">Call Count</span></span>
- <span data-ttu-id="66458-153">会议计数</span><span class="sxs-lookup"><span data-stu-id="66458-153">Meeting Count</span></span>
- <span data-ttu-id="66458-154">包含其他操作</span><span class="sxs-lookup"><span data-stu-id="66458-154">Has Other Action</span></span>
- <span data-ttu-id="66458-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="66458-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="66458-156">示例</span><span class="sxs-lookup"><span data-stu-id="66458-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="66458-157">请求</span><span class="sxs-lookup"><span data-stu-id="66458-157">Request</span></span>

<span data-ttu-id="66458-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="66458-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="66458-159">响应</span><span class="sxs-lookup"><span data-stu-id="66458-159">Response</span></span>

<span data-ttu-id="66458-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="66458-160">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="66458-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="66458-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66458-162">C#</span><span class="sxs-lookup"><span data-stu-id="66458-162">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66458-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="66458-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="66458-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="66458-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
