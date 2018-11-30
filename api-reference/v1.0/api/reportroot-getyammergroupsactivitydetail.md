---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: 获取组执行的 Yammer 组活动的详细信息。
ms.openlocfilehash: 927d9511a5190b2aa5540c6046c8162e5fa5f9e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009797"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="8421e-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="8421e-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="8421e-104">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8421e-104">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="8421e-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="8421e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="8421e-106">权限</span><span class="sxs-lookup"><span data-stu-id="8421e-106">Permissions</span></span>

<span data-ttu-id="8421e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8421e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8421e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8421e-109">Permission type</span></span>                        | <span data-ttu-id="8421e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8421e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="8421e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8421e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8421e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8421e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="8421e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8421e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8421e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8421e-114">Not supported.</span></span>                           |
| <span data-ttu-id="8421e-115">应用</span><span class="sxs-lookup"><span data-stu-id="8421e-115">Application</span></span>                            | <span data-ttu-id="8421e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="8421e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="8421e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8421e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="8421e-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="8421e-118">Function parameters</span></span>

<span data-ttu-id="8421e-119">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="8421e-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="8421e-120">参数</span><span class="sxs-lookup"><span data-stu-id="8421e-120">Parameter</span></span> | <span data-ttu-id="8421e-121">类型</span><span class="sxs-lookup"><span data-stu-id="8421e-121">Type</span></span>   | <span data-ttu-id="8421e-122">说明</span><span class="sxs-lookup"><span data-stu-id="8421e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="8421e-123">period</span><span class="sxs-lookup"><span data-stu-id="8421e-123">period</span></span>    | <span data-ttu-id="8421e-124">string</span><span class="sxs-lookup"><span data-stu-id="8421e-124">string</span></span> | <span data-ttu-id="8421e-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8421e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="8421e-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="8421e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="8421e-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="8421e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="8421e-128">date</span><span class="sxs-lookup"><span data-stu-id="8421e-128">date</span></span>      | <span data-ttu-id="8421e-129">Date</span><span class="sxs-lookup"><span data-stu-id="8421e-129">Date</span></span>   | <span data-ttu-id="8421e-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="8421e-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="8421e-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="8421e-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="8421e-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="8421e-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="8421e-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="8421e-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8421e-134">请求头</span><span class="sxs-lookup"><span data-stu-id="8421e-134">Request headers</span></span>

| <span data-ttu-id="8421e-135">名称</span><span class="sxs-lookup"><span data-stu-id="8421e-135">Name</span></span>          | <span data-ttu-id="8421e-136">说明</span><span class="sxs-lookup"><span data-stu-id="8421e-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="8421e-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="8421e-137">Authorization</span></span> | <span data-ttu-id="8421e-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="8421e-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="8421e-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="8421e-140">If-None-Match</span></span> | <span data-ttu-id="8421e-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8421e-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="8421e-142">可选。</span><span class="sxs-lookup"><span data-stu-id="8421e-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="8421e-143">响应</span><span class="sxs-lookup"><span data-stu-id="8421e-143">Response</span></span>

<span data-ttu-id="8421e-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="8421e-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="8421e-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="8421e-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="8421e-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="8421e-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="8421e-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="8421e-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="8421e-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="8421e-148">Report Refresh Date</span></span>
- <span data-ttu-id="8421e-149">组显示名称</span><span class="sxs-lookup"><span data-stu-id="8421e-149">Group Display Name</span></span>
- <span data-ttu-id="8421e-150">已删除</span><span class="sxs-lookup"><span data-stu-id="8421e-150">Is Deleted</span></span>
- <span data-ttu-id="8421e-151">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="8421e-151">Owner Principal Name</span></span>
- <span data-ttu-id="8421e-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="8421e-152">Last Activity Date</span></span>
- <span data-ttu-id="8421e-153">组类型</span><span class="sxs-lookup"><span data-stu-id="8421e-153">Group Type</span></span>
- <span data-ttu-id="8421e-154">Office 365 已连接</span><span class="sxs-lookup"><span data-stu-id="8421e-154">Office 365 Connected</span></span>
- <span data-ttu-id="8421e-155">成员数</span><span class="sxs-lookup"><span data-stu-id="8421e-155">Member Count</span></span>
- <span data-ttu-id="8421e-156">已发布数</span><span class="sxs-lookup"><span data-stu-id="8421e-156">Posted Count</span></span>
- <span data-ttu-id="8421e-157">已阅读数</span><span class="sxs-lookup"><span data-stu-id="8421e-157">Read Count</span></span>
- <span data-ttu-id="8421e-158">已赞数</span><span class="sxs-lookup"><span data-stu-id="8421e-158">Liked Count</span></span>
- <span data-ttu-id="8421e-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="8421e-159">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="8421e-160">示例</span><span class="sxs-lookup"><span data-stu-id="8421e-160">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8421e-161">请求</span><span class="sxs-lookup"><span data-stu-id="8421e-161">Request</span></span>

<span data-ttu-id="8421e-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8421e-162">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="8421e-163">响应</span><span class="sxs-lookup"><span data-stu-id="8421e-163">Response</span></span>

<span data-ttu-id="8421e-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8421e-164">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="8421e-165">请求</span><span class="sxs-lookup"><span data-stu-id="8421e-165">Request</span></span>
<span data-ttu-id="8421e-166">如果使用调用`date`，在指定日期范围到活动报告。</span><span class="sxs-lookup"><span data-stu-id="8421e-166">If called with a `date`, the report is scoped to activity on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammergroupsactivityuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerGroupsActivityDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="8421e-167">响应</span><span class="sxs-lookup"><span data-stu-id="8421e-167">Response</span></span>

<span data-ttu-id="8421e-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8421e-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="8421e-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="8421e-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "ignored"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```
