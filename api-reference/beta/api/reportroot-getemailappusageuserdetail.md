---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: 获取用户在不同电子邮件应用中执行的活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 4bbbc7cadac13134286c49aa58745c4f57a7c65c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050960"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="fa01e-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="fa01e-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="fa01e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa01e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa01e-105">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fa01e-105">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="fa01e-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报告 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="fa01e-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa01e-107">权限</span><span class="sxs-lookup"><span data-stu-id="fa01e-107">Permissions</span></span>

<span data-ttu-id="fa01e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa01e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa01e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa01e-110">Permission type</span></span>                        | <span data-ttu-id="fa01e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa01e-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fa01e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa01e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa01e-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa01e-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fa01e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa01e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa01e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa01e-115">Not supported.</span></span>                           |
| <span data-ttu-id="fa01e-116">应用</span><span class="sxs-lookup"><span data-stu-id="fa01e-116">Application</span></span>                            | <span data-ttu-id="fa01e-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa01e-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="fa01e-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="fa01e-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="fa01e-119">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="fa01e-119">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="fa01e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa01e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="fa01e-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="fa01e-121">Function parameters</span></span>

<span data-ttu-id="fa01e-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="fa01e-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="fa01e-123">参数</span><span class="sxs-lookup"><span data-stu-id="fa01e-123">Parameter</span></span> | <span data-ttu-id="fa01e-124">类型</span><span class="sxs-lookup"><span data-stu-id="fa01e-124">Type</span></span>   | <span data-ttu-id="fa01e-125">说明</span><span class="sxs-lookup"><span data-stu-id="fa01e-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fa01e-126">period</span><span class="sxs-lookup"><span data-stu-id="fa01e-126">period</span></span>    | <span data-ttu-id="fa01e-127">string</span><span class="sxs-lookup"><span data-stu-id="fa01e-127">string</span></span> | <span data-ttu-id="fa01e-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fa01e-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fa01e-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="fa01e-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fa01e-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fa01e-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="fa01e-131">date</span><span class="sxs-lookup"><span data-stu-id="fa01e-131">date</span></span>      | <span data-ttu-id="fa01e-132">Date</span><span class="sxs-lookup"><span data-stu-id="fa01e-132">Date</span></span>   | <span data-ttu-id="fa01e-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="fa01e-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="fa01e-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="fa01e-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="fa01e-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="fa01e-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="fa01e-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="fa01e-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="fa01e-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fa01e-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fa01e-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="fa01e-138">The default output type is text/csv.</span></span> <span data-ttu-id="fa01e-139">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="fa01e-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa01e-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa01e-140">Request headers</span></span>

| <span data-ttu-id="fa01e-141">名称</span><span class="sxs-lookup"><span data-stu-id="fa01e-141">Name</span></span>          | <span data-ttu-id="fa01e-142">说明</span><span class="sxs-lookup"><span data-stu-id="fa01e-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fa01e-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa01e-143">Authorization</span></span> | <span data-ttu-id="fa01e-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa01e-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fa01e-146">响应</span><span class="sxs-lookup"><span data-stu-id="fa01e-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fa01e-147">CSV</span><span class="sxs-lookup"><span data-stu-id="fa01e-147">CSV</span></span>

<span data-ttu-id="fa01e-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="fa01e-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fa01e-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="fa01e-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fa01e-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="fa01e-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fa01e-151">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="fa01e-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fa01e-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="fa01e-152">Report Refresh Date</span></span>
- <span data-ttu-id="fa01e-153">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="fa01e-153">User Principal Name</span></span>
- <span data-ttu-id="fa01e-154">显示名称</span><span class="sxs-lookup"><span data-stu-id="fa01e-154">Display Name</span></span>
- <span data-ttu-id="fa01e-155">已删除</span><span class="sxs-lookup"><span data-stu-id="fa01e-155">Is Deleted</span></span>
- <span data-ttu-id="fa01e-156">删除日期</span><span class="sxs-lookup"><span data-stu-id="fa01e-156">Deleted Date</span></span>
- <span data-ttu-id="fa01e-157">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="fa01e-157">Last Activity Date</span></span>
- <span data-ttu-id="fa01e-158">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="fa01e-158">Mail For Mac</span></span>
- <span data-ttu-id="fa01e-159">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="fa01e-159">Outlook For Mac</span></span>
- <span data-ttu-id="fa01e-160">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="fa01e-160">Outlook For Windows</span></span>
- <span data-ttu-id="fa01e-161">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="fa01e-161">Outlook For Mobile</span></span>
- <span data-ttu-id="fa01e-162">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="fa01e-162">Other For Mobile</span></span>
- <span data-ttu-id="fa01e-163">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="fa01e-163">Outlook For Web</span></span>
- <span data-ttu-id="fa01e-164">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="fa01e-164">POP3 App</span></span>
- <span data-ttu-id="fa01e-165">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="fa01e-165">IMAP4 App</span></span>
- <span data-ttu-id="fa01e-166">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="fa01e-166">SMTP App</span></span>
- <span data-ttu-id="fa01e-167">报表周期</span><span class="sxs-lookup"><span data-stu-id="fa01e-167">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fa01e-168">JSON</span><span class="sxs-lookup"><span data-stu-id="fa01e-168">JSON</span></span>

<span data-ttu-id="fa01e-169">如果成功，此方法在响应 `200 OK` 正文中返回 响应 **[代码和 emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="fa01e-169">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="fa01e-170">此请求的默认页面大小为 200 个项目。</span><span class="sxs-lookup"><span data-stu-id="fa01e-170">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="fa01e-171">示例</span><span class="sxs-lookup"><span data-stu-id="fa01e-171">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fa01e-172">CSV</span><span class="sxs-lookup"><span data-stu-id="fa01e-172">CSV</span></span>

<span data-ttu-id="fa01e-173">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="fa01e-173">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fa01e-174">请求</span><span class="sxs-lookup"><span data-stu-id="fa01e-174">Request</span></span>

<span data-ttu-id="fa01e-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fa01e-175">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="fa01e-176">响应</span><span class="sxs-lookup"><span data-stu-id="fa01e-176">Response</span></span>

<span data-ttu-id="fa01e-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fa01e-177">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fa01e-178">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="fa01e-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="fa01e-179">JSON</span><span class="sxs-lookup"><span data-stu-id="fa01e-179">JSON</span></span>

<span data-ttu-id="fa01e-180">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="fa01e-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fa01e-181">请求</span><span class="sxs-lookup"><span data-stu-id="fa01e-181">Request</span></span>

<span data-ttu-id="fa01e-182">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fa01e-182">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="fa01e-183">响应</span><span class="sxs-lookup"><span data-stu-id="fa01e-183">Response</span></span>

<span data-ttu-id="fa01e-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fa01e-184">The following is an example of the response.</span></span>

> <span data-ttu-id="fa01e-185">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fa01e-185">**Note:** The response object shown here might be shortened for readability.</span></span>

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


