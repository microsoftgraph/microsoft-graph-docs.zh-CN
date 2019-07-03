---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: 获取用户在不同电子邮件应用中执行的活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bde1a3de90796dda65fc9d227fe0432df2ded47c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449419"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="e3fb3-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="e3fb3-103">reportRoot: getEmailAppUsageUserDetail</span></span>

<span data-ttu-id="e3fb3-104">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="e3fb3-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3fb3-106">权限</span><span class="sxs-lookup"><span data-stu-id="e3fb3-106">Permissions</span></span>

<span data-ttu-id="e3fb3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3fb3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3fb3-109">Permission type</span></span>                        | <span data-ttu-id="e3fb3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3fb3-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e3fb3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3fb3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3fb3-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3fb3-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e3fb3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3fb3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3fb3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-114">Not supported.</span></span>                           |
| <span data-ttu-id="e3fb3-115">应用</span><span class="sxs-lookup"><span data-stu-id="e3fb3-115">Application</span></span>                            | <span data-ttu-id="e3fb3-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3fb3-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e3fb3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3fb3-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e3fb3-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e3fb3-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e3fb3-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="e3fb3-119">Function parameters</span></span>

<span data-ttu-id="e3fb3-120">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e3fb3-121">参数</span><span class="sxs-lookup"><span data-stu-id="e3fb3-121">Parameter</span></span> | <span data-ttu-id="e3fb3-122">类型</span><span class="sxs-lookup"><span data-stu-id="e3fb3-122">Type</span></span>   | <span data-ttu-id="e3fb3-123">说明</span><span class="sxs-lookup"><span data-stu-id="e3fb3-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e3fb3-124">period</span><span class="sxs-lookup"><span data-stu-id="e3fb3-124">period</span></span>    | <span data-ttu-id="e3fb3-125">string</span><span class="sxs-lookup"><span data-stu-id="e3fb3-125">string</span></span> | <span data-ttu-id="e3fb3-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e3fb3-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e3fb3-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e3fb3-129">date</span><span class="sxs-lookup"><span data-stu-id="e3fb3-129">date</span></span>      | <span data-ttu-id="e3fb3-130">Date</span><span class="sxs-lookup"><span data-stu-id="e3fb3-130">Date</span></span>   | <span data-ttu-id="e3fb3-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e3fb3-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e3fb3-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e3fb3-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3fb3-135">请求头</span><span class="sxs-lookup"><span data-stu-id="e3fb3-135">Request headers</span></span>

| <span data-ttu-id="e3fb3-136">名称</span><span class="sxs-lookup"><span data-stu-id="e3fb3-136">Name</span></span>          | <span data-ttu-id="e3fb3-137">说明</span><span class="sxs-lookup"><span data-stu-id="e3fb3-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="e3fb3-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3fb3-138">Authorization</span></span> | <span data-ttu-id="e3fb3-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="e3fb3-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="e3fb3-141">If-None-Match</span></span> | <span data-ttu-id="e3fb3-142">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="e3fb3-143">可选。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="e3fb3-144">响应</span><span class="sxs-lookup"><span data-stu-id="e3fb3-144">Response</span></span>

<span data-ttu-id="e3fb3-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e3fb3-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e3fb3-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e3fb3-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e3fb3-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e3fb3-149">Report Refresh Date</span></span>
- <span data-ttu-id="e3fb3-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e3fb3-150">User Principal Name</span></span>
- <span data-ttu-id="e3fb3-151">显示名称</span><span class="sxs-lookup"><span data-stu-id="e3fb3-151">Display Name</span></span>
- <span data-ttu-id="e3fb3-152">已删除</span><span class="sxs-lookup"><span data-stu-id="e3fb3-152">Is Deleted</span></span>
- <span data-ttu-id="e3fb3-153">删除日期</span><span class="sxs-lookup"><span data-stu-id="e3fb3-153">Deleted Date</span></span>
- <span data-ttu-id="e3fb3-154">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e3fb3-154">Last Activity Date</span></span>
- <span data-ttu-id="e3fb3-155">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="e3fb3-155">Mail For Mac</span></span>
- <span data-ttu-id="e3fb3-156">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="e3fb3-156">Outlook For Mac</span></span>
- <span data-ttu-id="e3fb3-157">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="e3fb3-157">Outlook For Windows</span></span>
- <span data-ttu-id="e3fb3-158">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="e3fb3-158">Outlook For Mobile</span></span>
- <span data-ttu-id="e3fb3-159">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="e3fb3-159">Other For Mobile</span></span>
- <span data-ttu-id="e3fb3-160">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="e3fb3-160">Outlook For Web</span></span>
- <span data-ttu-id="e3fb3-161">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="e3fb3-161">POP3 App</span></span>
- <span data-ttu-id="e3fb3-162">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="e3fb3-162">IMAP4 App</span></span>
- <span data-ttu-id="e3fb3-163">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="e3fb3-163">SMTP App</span></span>
- <span data-ttu-id="e3fb3-164">报表周期</span><span class="sxs-lookup"><span data-stu-id="e3fb3-164">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="e3fb3-165">示例</span><span class="sxs-lookup"><span data-stu-id="e3fb3-165">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e3fb3-166">请求</span><span class="sxs-lookup"><span data-stu-id="e3fb3-166">Request</span></span>

<span data-ttu-id="e3fb3-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-167">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e3fb3-168">C#</span><span class="sxs-lookup"><span data-stu-id="e3fb3-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3fb3-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3fb3-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e3fb3-170">目标-C</span><span class="sxs-lookup"><span data-stu-id="e3fb3-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e3fb3-171">响应</span><span class="sxs-lookup"><span data-stu-id="e3fb3-171">Response</span></span>

<span data-ttu-id="e3fb3-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-172">The following is an example of the response.</span></span>

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

<span data-ttu-id="e3fb3-173">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e3fb3-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
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
