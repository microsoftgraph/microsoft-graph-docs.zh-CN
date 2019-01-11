---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: 获取用户在不同电子邮件应用中执行的活动的详细信息。
localization_priority: Normal
ms.openlocfilehash: a00dae579d90ae705c0c63d7d37065c9bf7850f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876907"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="1ee92-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="1ee92-103">reportRoot: getEmailAppUsageUserDetail</span></span>

> <span data-ttu-id="1ee92-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1ee92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ee92-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1ee92-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1ee92-106">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1ee92-106">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="1ee92-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="1ee92-107">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="1ee92-108">权限</span><span class="sxs-lookup"><span data-stu-id="1ee92-108">Permissions</span></span>

<span data-ttu-id="1ee92-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ee92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ee92-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ee92-111">Permission type</span></span>                        | <span data-ttu-id="1ee92-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ee92-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1ee92-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ee92-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ee92-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ee92-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1ee92-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ee92-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ee92-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ee92-116">Not supported.</span></span>                           |
| <span data-ttu-id="1ee92-117">应用</span><span class="sxs-lookup"><span data-stu-id="1ee92-117">Application</span></span>                            | <span data-ttu-id="1ee92-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ee92-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1ee92-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ee92-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="1ee92-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="1ee92-120">Function parameters</span></span>

<span data-ttu-id="1ee92-121">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="1ee92-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="1ee92-122">参数</span><span class="sxs-lookup"><span data-stu-id="1ee92-122">Parameter</span></span> | <span data-ttu-id="1ee92-123">类型</span><span class="sxs-lookup"><span data-stu-id="1ee92-123">Type</span></span>   | <span data-ttu-id="1ee92-124">说明</span><span class="sxs-lookup"><span data-stu-id="1ee92-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1ee92-125">period</span><span class="sxs-lookup"><span data-stu-id="1ee92-125">period</span></span>    | <span data-ttu-id="1ee92-126">string</span><span class="sxs-lookup"><span data-stu-id="1ee92-126">string</span></span> | <span data-ttu-id="1ee92-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1ee92-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1ee92-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="1ee92-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1ee92-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1ee92-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1ee92-130">date</span><span class="sxs-lookup"><span data-stu-id="1ee92-130">date</span></span>      | <span data-ttu-id="1ee92-131">Date</span><span class="sxs-lookup"><span data-stu-id="1ee92-131">Date</span></span>   | <span data-ttu-id="1ee92-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="1ee92-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1ee92-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="1ee92-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1ee92-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="1ee92-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1ee92-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="1ee92-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="1ee92-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1ee92-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1ee92-137">默认输出类型是文本/csv。</span><span class="sxs-lookup"><span data-stu-id="1ee92-137">The default output type is text/csv.</span></span> <span data-ttu-id="1ee92-138">但是，如果您想要指定输出类型，您可以使用 OData $format 查询参数设置为 text/csv 或应用程序/json。</span><span class="sxs-lookup"><span data-stu-id="1ee92-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ee92-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ee92-139">Request headers</span></span>

| <span data-ttu-id="1ee92-140">名称</span><span class="sxs-lookup"><span data-stu-id="1ee92-140">Name</span></span>          | <span data-ttu-id="1ee92-141">说明</span><span class="sxs-lookup"><span data-stu-id="1ee92-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1ee92-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ee92-142">Authorization</span></span> | <span data-ttu-id="1ee92-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ee92-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1ee92-145">响应</span><span class="sxs-lookup"><span data-stu-id="1ee92-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1ee92-146">CSV</span><span class="sxs-lookup"><span data-stu-id="1ee92-146">CSV</span></span>

<span data-ttu-id="1ee92-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="1ee92-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1ee92-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="1ee92-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1ee92-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="1ee92-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1ee92-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="1ee92-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1ee92-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="1ee92-151">Report Refresh Date</span></span>
- <span data-ttu-id="1ee92-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="1ee92-152">User Principal Name</span></span>
- <span data-ttu-id="1ee92-153">显示名称</span><span class="sxs-lookup"><span data-stu-id="1ee92-153">Display Name</span></span>
- <span data-ttu-id="1ee92-154">已删除</span><span class="sxs-lookup"><span data-stu-id="1ee92-154">Is Deleted</span></span>
- <span data-ttu-id="1ee92-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="1ee92-155">Deleted Date</span></span>
- <span data-ttu-id="1ee92-156">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="1ee92-156">Last Activity Date</span></span>
- <span data-ttu-id="1ee92-157">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="1ee92-157">Mail For Mac</span></span>
- <span data-ttu-id="1ee92-158">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="1ee92-158">Outlook For Mac</span></span>
- <span data-ttu-id="1ee92-159">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="1ee92-159">Outlook For Windows</span></span>
- <span data-ttu-id="1ee92-160">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="1ee92-160">Outlook For Mobile</span></span>
- <span data-ttu-id="1ee92-161">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="1ee92-161">Other For Mobile</span></span>
- <span data-ttu-id="1ee92-162">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="1ee92-162">Outlook For Web</span></span>
- <span data-ttu-id="1ee92-163">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="1ee92-163">POP3 App</span></span>
- <span data-ttu-id="1ee92-164">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="1ee92-164">IMAP4 App</span></span>
- <span data-ttu-id="1ee92-165">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="1ee92-165">SMTP App</span></span>
- <span data-ttu-id="1ee92-166">报表周期</span><span class="sxs-lookup"><span data-stu-id="1ee92-166">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1ee92-167">JSON</span><span class="sxs-lookup"><span data-stu-id="1ee92-167">JSON</span></span>

<span data-ttu-id="1ee92-168">如果成功，此方法返回`200 OK`响应代码和响应正文中的**[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="1ee92-168">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="1ee92-169">为此请求的默认页面大小是 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="1ee92-169">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="1ee92-170">示例</span><span class="sxs-lookup"><span data-stu-id="1ee92-170">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1ee92-171">CSV</span><span class="sxs-lookup"><span data-stu-id="1ee92-171">CSV</span></span>

<span data-ttu-id="1ee92-172">下面是输出 CSV 示例。</span><span class="sxs-lookup"><span data-stu-id="1ee92-172">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1ee92-173">请求</span><span class="sxs-lookup"><span data-stu-id="1ee92-173">Request</span></span>

<span data-ttu-id="1ee92-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ee92-174">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1ee92-175">响应</span><span class="sxs-lookup"><span data-stu-id="1ee92-175">Response</span></span>

<span data-ttu-id="1ee92-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ee92-176">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="1ee92-177">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="1ee92-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="1ee92-178">JSON</span><span class="sxs-lookup"><span data-stu-id="1ee92-178">JSON</span></span>

<span data-ttu-id="1ee92-179">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="1ee92-179">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1ee92-180">请求</span><span class="sxs-lookup"><span data-stu-id="1ee92-180">Request</span></span>

<span data-ttu-id="1ee92-181">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ee92-181">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1ee92-182">响应</span><span class="sxs-lookup"><span data-stu-id="1ee92-182">Response</span></span>

<span data-ttu-id="1ee92-183">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ee92-183">The following is an example of the response.</span></span>

> <span data-ttu-id="1ee92-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1ee92-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "mailForMac": [ ], 
      "outlookForMac": [ ], 
      "outlookForWindows": [ ], 
      "outlookForMobile": [
        "Undetermined"
      ], 
      "otherForMobile": [ ], 
      "outlookForWeb": [
        "Undetermined"
      ], 
      "pop3App": [ ], 
      "imap4App": [ ], 
      "smtpApp": [ ], 
      "reportPeriod": "7"
    }
  ]
}
```
