---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: 获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7821b321a28a81868147b00314c8ca774f8b75f0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33606970"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="3c03e-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3c03e-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="3c03e-104">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="3c03e-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="3c03e-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="3c03e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c03e-106">权限</span><span class="sxs-lookup"><span data-stu-id="3c03e-106">Permissions</span></span>

<span data-ttu-id="3c03e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c03e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c03e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c03e-109">Permission type</span></span>                        | <span data-ttu-id="3c03e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c03e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3c03e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c03e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c03e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c03e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3c03e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c03e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c03e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c03e-114">Not supported.</span></span>                           |
| <span data-ttu-id="3c03e-115">应用</span><span class="sxs-lookup"><span data-stu-id="3c03e-115">Application</span></span>                            | <span data-ttu-id="3c03e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c03e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3c03e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c03e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3c03e-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="3c03e-118">Function parameters</span></span>

<span data-ttu-id="3c03e-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="3c03e-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3c03e-120">参数</span><span class="sxs-lookup"><span data-stu-id="3c03e-120">Parameter</span></span> | <span data-ttu-id="3c03e-121">类型</span><span class="sxs-lookup"><span data-stu-id="3c03e-121">Type</span></span>   | <span data-ttu-id="3c03e-122">说明</span><span class="sxs-lookup"><span data-stu-id="3c03e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3c03e-123">period</span><span class="sxs-lookup"><span data-stu-id="3c03e-123">period</span></span>    | <span data-ttu-id="3c03e-124">string</span><span class="sxs-lookup"><span data-stu-id="3c03e-124">string</span></span> | <span data-ttu-id="3c03e-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3c03e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3c03e-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="3c03e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3c03e-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3c03e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3c03e-128">必需。</span><span class="sxs-lookup"><span data-stu-id="3c03e-128">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="3c03e-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c03e-129">Request headers</span></span>

| <span data-ttu-id="3c03e-130">名称</span><span class="sxs-lookup"><span data-stu-id="3c03e-130">Name</span></span>          | <span data-ttu-id="3c03e-131">说明</span><span class="sxs-lookup"><span data-stu-id="3c03e-131">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="3c03e-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c03e-132">Authorization</span></span> | <span data-ttu-id="3c03e-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c03e-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="3c03e-135">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="3c03e-135">If-None-Match</span></span> | <span data-ttu-id="3c03e-136">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3c03e-136">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="3c03e-137">可选。</span><span class="sxs-lookup"><span data-stu-id="3c03e-137">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="3c03e-138">响应</span><span class="sxs-lookup"><span data-stu-id="3c03e-138">Response</span></span>

<span data-ttu-id="3c03e-139">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3c03e-139">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3c03e-140">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="3c03e-140">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3c03e-141">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="3c03e-141">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3c03e-142">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="3c03e-142">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3c03e-143">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="3c03e-143">Report Refresh Date</span></span>
- <span data-ttu-id="3c03e-144">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="3c03e-144">Mail For Mac</span></span>
- <span data-ttu-id="3c03e-145">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="3c03e-145">Outlook For Mac</span></span>
- <span data-ttu-id="3c03e-146">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="3c03e-146">Outlook For Windows</span></span>
- <span data-ttu-id="3c03e-147">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="3c03e-147">Outlook For Mobile</span></span>
- <span data-ttu-id="3c03e-148">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="3c03e-148">Other For Mobile</span></span>
- <span data-ttu-id="3c03e-149">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="3c03e-149">Outlook For Web</span></span>
- <span data-ttu-id="3c03e-150">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="3c03e-150">POP3 App</span></span>
- <span data-ttu-id="3c03e-151">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="3c03e-151">IMAP4 App</span></span>
- <span data-ttu-id="3c03e-152">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="3c03e-152">SMTP App</span></span>
- <span data-ttu-id="3c03e-153">报表日期</span><span class="sxs-lookup"><span data-stu-id="3c03e-153">Report Date</span></span>
- <span data-ttu-id="3c03e-154">报表周期</span><span class="sxs-lookup"><span data-stu-id="3c03e-154">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="3c03e-155">示例</span><span class="sxs-lookup"><span data-stu-id="3c03e-155">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3c03e-156">请求</span><span class="sxs-lookup"><span data-stu-id="3c03e-156">Request</span></span>

<span data-ttu-id="3c03e-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3c03e-157">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="3c03e-158">响应</span><span class="sxs-lookup"><span data-stu-id="3c03e-158">Response</span></span>

<span data-ttu-id="3c03e-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3c03e-159">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3c03e-160">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3c03e-160">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3c03e-161">语言</span><span class="sxs-lookup"><span data-stu-id="3c03e-161">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c03e-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c03e-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="3c03e-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="3c03e-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
