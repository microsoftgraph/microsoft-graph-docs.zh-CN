---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: 获取用户的 Yammer 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 140d5cd4ab56d8509ebd411b99c7a08de1ac44da
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787770"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="5b6c0-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="5b6c0-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

<span data-ttu-id="5b6c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b6c0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b6c0-105">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-105">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="5b6c0-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报表 -](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)Yammer使用情况。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="5b6c0-107">权限</span><span class="sxs-lookup"><span data-stu-id="5b6c0-107">Permissions</span></span>

<span data-ttu-id="5b6c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b6c0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b6c0-110">Permission type</span></span>                        | <span data-ttu-id="5b6c0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b6c0-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5b6c0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b6c0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b6c0-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b6c0-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5b6c0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b6c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b6c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-115">Not supported.</span></span>                           |
| <span data-ttu-id="5b6c0-116">应用</span><span class="sxs-lookup"><span data-stu-id="5b6c0-116">Application</span></span>                            | <span data-ttu-id="5b6c0-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b6c0-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="5b6c0-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5b6c0-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5b6c0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b6c0-120">HTTP request</span></span>


<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5b6c0-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="5b6c0-121">Function parameters</span></span>

<span data-ttu-id="5b6c0-122">在请求 URL 中，提供查询参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-122">In the request URL, provide the query parameter with a valid value.</span></span>

| <span data-ttu-id="5b6c0-123">参数</span><span class="sxs-lookup"><span data-stu-id="5b6c0-123">Parameter</span></span> | <span data-ttu-id="5b6c0-124">类型</span><span class="sxs-lookup"><span data-stu-id="5b6c0-124">Type</span></span>   | <span data-ttu-id="5b6c0-125">说明</span><span class="sxs-lookup"><span data-stu-id="5b6c0-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5b6c0-126">period</span><span class="sxs-lookup"><span data-stu-id="5b6c0-126">period</span></span>    | <span data-ttu-id="5b6c0-127">string</span><span class="sxs-lookup"><span data-stu-id="5b6c0-127">string</span></span> | <span data-ttu-id="5b6c0-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5b6c0-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5b6c0-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5b6c0-131">date</span><span class="sxs-lookup"><span data-stu-id="5b6c0-131">date</span></span>      | <span data-ttu-id="5b6c0-132">Date</span><span class="sxs-lookup"><span data-stu-id="5b6c0-132">Date</span></span>   | <span data-ttu-id="5b6c0-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5b6c0-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5b6c0-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5b6c0-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-136">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b6c0-137">请求头</span><span class="sxs-lookup"><span data-stu-id="5b6c0-137">Request headers</span></span>

| <span data-ttu-id="5b6c0-138">名称</span><span class="sxs-lookup"><span data-stu-id="5b6c0-138">Name</span></span>          | <span data-ttu-id="5b6c0-139">说明</span><span class="sxs-lookup"><span data-stu-id="5b6c0-139">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5b6c0-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b6c0-140">Authorization</span></span> | <span data-ttu-id="5b6c0-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5b6c0-143">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5b6c0-143">If-None-Match</span></span> | <span data-ttu-id="5b6c0-144">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-144">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5b6c0-145">可选。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-145">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5b6c0-146">响应</span><span class="sxs-lookup"><span data-stu-id="5b6c0-146">Response</span></span>

<span data-ttu-id="5b6c0-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5b6c0-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5b6c0-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5b6c0-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5b6c0-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="5b6c0-151">Report Refresh Date</span></span>
- <span data-ttu-id="5b6c0-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="5b6c0-152">User Principal Name</span></span>
- <span data-ttu-id="5b6c0-153">显示名称</span><span class="sxs-lookup"><span data-stu-id="5b6c0-153">Display Name</span></span>
- <span data-ttu-id="5b6c0-154">用户状态</span><span class="sxs-lookup"><span data-stu-id="5b6c0-154">User State</span></span>
- <span data-ttu-id="5b6c0-155">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="5b6c0-155">State Change Date</span></span>
- <span data-ttu-id="5b6c0-156">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="5b6c0-156">Last Activity Date</span></span>
- <span data-ttu-id="5b6c0-157">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="5b6c0-157">Used Web</span></span>
- <span data-ttu-id="5b6c0-158">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="5b6c0-158">Used Windows Phone</span></span>
- <span data-ttu-id="5b6c0-159">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="5b6c0-159">Used Android Phone</span></span>
- <span data-ttu-id="5b6c0-160">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="5b6c0-160">Used iPhone</span></span>
- <span data-ttu-id="5b6c0-161">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="5b6c0-161">Used iPad</span></span>
- <span data-ttu-id="5b6c0-162">使用的其他设备</span><span class="sxs-lookup"><span data-stu-id="5b6c0-162">Used Others</span></span>
- <span data-ttu-id="5b6c0-163">报表周期</span><span class="sxs-lookup"><span data-stu-id="5b6c0-163">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5b6c0-164">示例</span><span class="sxs-lookup"><span data-stu-id="5b6c0-164">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5b6c0-165">请求</span><span class="sxs-lookup"><span data-stu-id="5b6c0-165">Request</span></span>

<span data-ttu-id="5b6c0-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-166">The following is an example of the request.</span></span>


<!--{
  "blockType": "ignored",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(period='D7')
```


#### <a name="response"></a><span data-ttu-id="5b6c0-167">响应</span><span class="sxs-lookup"><span data-stu-id="5b6c0-167">Response</span></span>

<span data-ttu-id="5b6c0-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-168">The following is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.report" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

#### <a name="request"></a><span data-ttu-id="5b6c0-169">请求</span><span class="sxs-lookup"><span data-stu-id="5b6c0-169">Request</span></span>

<span data-ttu-id="5b6c0-170">如果使用 参数 `date` 调用，则报告的范围为给定日期的使用范围。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-170">If called with the `date` parameter, the report is scoped to usage on the given date.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getyammerdeviceusageuserdetail_date"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getYammerDeviceUsageUserDetail(date='2018-03-05')
```

#### <a name="response"></a><span data-ttu-id="5b6c0-171">响应</span><span class="sxs-lookup"><span data-stu-id="5b6c0-171">Response</span></span>

<span data-ttu-id="5b6c0-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5b6c0-173">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="5b6c0-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
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

