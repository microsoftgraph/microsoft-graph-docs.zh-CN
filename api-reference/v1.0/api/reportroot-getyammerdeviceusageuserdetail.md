---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: 获取用户的 Yammer 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: d273c2102226f75ff0638402b534511003b0102f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571420"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="2fa7c-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="2fa7c-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="2fa7c-104">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="2fa7c-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="2fa7c-106">权限</span><span class="sxs-lookup"><span data-stu-id="2fa7c-106">Permissions</span></span>

<span data-ttu-id="2fa7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fa7c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fa7c-109">Permission type</span></span>                        | <span data-ttu-id="2fa7c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2fa7c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2fa7c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fa7c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2fa7c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fa7c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2fa7c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fa7c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fa7c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-114">Not supported.</span></span>                           |
| <span data-ttu-id="2fa7c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fa7c-115">Application</span></span>                            | <span data-ttu-id="2fa7c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fa7c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2fa7c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fa7c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="2fa7c-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="2fa7c-118">Function parameters</span></span>

<span data-ttu-id="2fa7c-119">在请求 URL 中，提供查询参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-119">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="2fa7c-120">参数</span><span class="sxs-lookup"><span data-stu-id="2fa7c-120">Parameter</span></span> | <span data-ttu-id="2fa7c-121">类型</span><span class="sxs-lookup"><span data-stu-id="2fa7c-121">Type</span></span>   | <span data-ttu-id="2fa7c-122">说明</span><span class="sxs-lookup"><span data-stu-id="2fa7c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2fa7c-123">period</span><span class="sxs-lookup"><span data-stu-id="2fa7c-123">period</span></span>    | <span data-ttu-id="2fa7c-124">string</span><span class="sxs-lookup"><span data-stu-id="2fa7c-124">string</span></span> | <span data-ttu-id="2fa7c-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2fa7c-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2fa7c-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2fa7c-128">date</span><span class="sxs-lookup"><span data-stu-id="2fa7c-128">date</span></span>      | <span data-ttu-id="2fa7c-129">Date</span><span class="sxs-lookup"><span data-stu-id="2fa7c-129">Date</span></span>   | <span data-ttu-id="2fa7c-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2fa7c-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2fa7c-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="2fa7c-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2fa7c-134">请求头</span><span class="sxs-lookup"><span data-stu-id="2fa7c-134">Request headers</span></span>

| <span data-ttu-id="2fa7c-135">名称</span><span class="sxs-lookup"><span data-stu-id="2fa7c-135">Name</span></span>          | <span data-ttu-id="2fa7c-136">说明</span><span class="sxs-lookup"><span data-stu-id="2fa7c-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2fa7c-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fa7c-137">Authorization</span></span> | <span data-ttu-id="2fa7c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2fa7c-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2fa7c-140">If-None-Match</span></span> | <span data-ttu-id="2fa7c-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2fa7c-142">可选。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2fa7c-143">响应</span><span class="sxs-lookup"><span data-stu-id="2fa7c-143">Response</span></span>

<span data-ttu-id="2fa7c-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2fa7c-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2fa7c-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2fa7c-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2fa7c-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2fa7c-148">Report Refresh Date</span></span>
- <span data-ttu-id="2fa7c-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="2fa7c-149">User Principal Name</span></span>
- <span data-ttu-id="2fa7c-150">显示名称</span><span class="sxs-lookup"><span data-stu-id="2fa7c-150">Display Name</span></span>
- <span data-ttu-id="2fa7c-151">用户状态</span><span class="sxs-lookup"><span data-stu-id="2fa7c-151">User State</span></span>
- <span data-ttu-id="2fa7c-152">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="2fa7c-152">State Change Date</span></span>
- <span data-ttu-id="2fa7c-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="2fa7c-153">Last Activity Date</span></span>
- <span data-ttu-id="2fa7c-154">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="2fa7c-154">Used Web</span></span>
- <span data-ttu-id="2fa7c-155">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="2fa7c-155">Used Windows Phone</span></span>
- <span data-ttu-id="2fa7c-156">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="2fa7c-156">Used Android Phone</span></span>
- <span data-ttu-id="2fa7c-157">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="2fa7c-157">Used iPhone</span></span>
- <span data-ttu-id="2fa7c-158">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="2fa7c-158">Used iPad</span></span>
- <span data-ttu-id="2fa7c-159">使用的其他设备</span><span class="sxs-lookup"><span data-stu-id="2fa7c-159">Used Others</span></span>
- <span data-ttu-id="2fa7c-160">报表周期</span><span class="sxs-lookup"><span data-stu-id="2fa7c-160">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2fa7c-161">示例</span><span class="sxs-lookup"><span data-stu-id="2fa7c-161">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2fa7c-162">请求</span><span class="sxs-lookup"><span data-stu-id="2fa7c-162">Request</span></span>

<span data-ttu-id="2fa7c-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-163">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="2fa7c-164">响应</span><span class="sxs-lookup"><span data-stu-id="2fa7c-164">Response</span></span>

<span data-ttu-id="2fa7c-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-165">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="2fa7c-166">请求</span><span class="sxs-lookup"><span data-stu-id="2fa7c-166">Request</span></span>

<span data-ttu-id="2fa7c-167">如果使用`date`参数调用, 则报告的作用范围为给定日期的使用情况。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-167">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="2fa7c-168">响应</span><span class="sxs-lookup"><span data-stu-id="2fa7c-168">Response</span></span>

<span data-ttu-id="2fa7c-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-169">The following is an example of the response.</span></span>

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

<span data-ttu-id="2fa7c-170">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2fa7c-170">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```
