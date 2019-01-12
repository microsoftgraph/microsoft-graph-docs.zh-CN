---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: 按用户获取有关 Microsoft Teams 用户活动的详细信息。
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: b968a5cb17ad588ffea678b05a5752e226b5eb5d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960705"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="62898-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="62898-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="62898-104">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="62898-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="62898-105">权限</span><span class="sxs-lookup"><span data-stu-id="62898-105">Permissions</span></span>

<span data-ttu-id="62898-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62898-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="62898-108">Permission type</span></span>                        | <span data-ttu-id="62898-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62898-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="62898-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62898-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="62898-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62898-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="62898-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62898-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62898-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="62898-113">Not supported.</span></span>                           |
| <span data-ttu-id="62898-114">应用</span><span class="sxs-lookup"><span data-stu-id="62898-114">Application</span></span>                            | <span data-ttu-id="62898-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="62898-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="62898-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62898-116">HTTP request</span></span>

<!-- { "blockType": "samples" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='{period_value}')
GET /reports/getTeamsUserActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="62898-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="62898-117">Function parameters</span></span>

<span data-ttu-id="62898-118">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="62898-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="62898-119">参数</span><span class="sxs-lookup"><span data-stu-id="62898-119">Parameter</span></span> | <span data-ttu-id="62898-120">类型</span><span class="sxs-lookup"><span data-stu-id="62898-120">Type</span></span>   | <span data-ttu-id="62898-121">说明</span><span class="sxs-lookup"><span data-stu-id="62898-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="62898-122">period</span><span class="sxs-lookup"><span data-stu-id="62898-122">period</span></span>    | <span data-ttu-id="62898-123">string</span><span class="sxs-lookup"><span data-stu-id="62898-123">string</span></span> | <span data-ttu-id="62898-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="62898-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="62898-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="62898-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="62898-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="62898-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="62898-127">date</span><span class="sxs-lookup"><span data-stu-id="62898-127">date</span></span>      | <span data-ttu-id="62898-128">Date</span><span class="sxs-lookup"><span data-stu-id="62898-128">Date</span></span>   | <span data-ttu-id="62898-129">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="62898-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="62898-130">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="62898-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="62898-131">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="62898-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="62898-132">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="62898-132">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="62898-133">请求头</span><span class="sxs-lookup"><span data-stu-id="62898-133">Request headers</span></span>

| <span data-ttu-id="62898-134">名称</span><span class="sxs-lookup"><span data-stu-id="62898-134">Name</span></span>          | <span data-ttu-id="62898-135">说明</span><span class="sxs-lookup"><span data-stu-id="62898-135">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="62898-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="62898-136">Authorization</span></span> | <span data-ttu-id="62898-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62898-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="62898-139">响应</span><span class="sxs-lookup"><span data-stu-id="62898-139">Response</span></span>

<span data-ttu-id="62898-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="62898-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="62898-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="62898-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="62898-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="62898-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="62898-143">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="62898-143">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="62898-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="62898-144">Report Refresh Date</span></span>
- <span data-ttu-id="62898-145">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="62898-145">User Principal Name</span></span>
- <span data-ttu-id="62898-146">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="62898-146">Last Activity Date</span></span>
- <span data-ttu-id="62898-147">已删除</span><span class="sxs-lookup"><span data-stu-id="62898-147">Is Deleted</span></span>
- <span data-ttu-id="62898-148">删除日期</span><span class="sxs-lookup"><span data-stu-id="62898-148">Deleted Date</span></span>
- <span data-ttu-id="62898-149">分配的产品</span><span class="sxs-lookup"><span data-stu-id="62898-149">Assigned Products</span></span>
- <span data-ttu-id="62898-150">团队聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="62898-150">Team Chat Message Count</span></span>
- <span data-ttu-id="62898-151">专用聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="62898-151">Private Chat Message Count</span></span>
- <span data-ttu-id="62898-152">呼叫计数</span><span class="sxs-lookup"><span data-stu-id="62898-152">Call Count</span></span>
- <span data-ttu-id="62898-153">会议计数</span><span class="sxs-lookup"><span data-stu-id="62898-153">Meeting Count</span></span>
- <span data-ttu-id="62898-154">包含其他操作</span><span class="sxs-lookup"><span data-stu-id="62898-154">Has Other Action</span></span>
- <span data-ttu-id="62898-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="62898-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="62898-156">示例</span><span class="sxs-lookup"><span data-stu-id="62898-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="62898-157">请求</span><span class="sxs-lookup"><span data-stu-id="62898-157">Request</span></span>

<span data-ttu-id="62898-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62898-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getTeamsUserActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="62898-159">响应</span><span class="sxs-lookup"><span data-stu-id="62898-159">Response</span></span>

<span data-ttu-id="62898-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62898-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="62898-161">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="62898-161">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```
