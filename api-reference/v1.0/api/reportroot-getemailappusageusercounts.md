---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: 获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: e987c82b94159bcecd19638f4c8e1d56e538c3cb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449426"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="2106d-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="2106d-103">reportRoot: getEmailAppUsageUserCounts</span></span>

<span data-ttu-id="2106d-104">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="2106d-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="2106d-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="2106d-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="2106d-106">权限</span><span class="sxs-lookup"><span data-stu-id="2106d-106">Permissions</span></span>

<span data-ttu-id="2106d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2106d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2106d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2106d-109">Permission type</span></span>                        | <span data-ttu-id="2106d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2106d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2106d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2106d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2106d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2106d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2106d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2106d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2106d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2106d-114">Not supported.</span></span>                           |
| <span data-ttu-id="2106d-115">应用</span><span class="sxs-lookup"><span data-stu-id="2106d-115">Application</span></span>                            | <span data-ttu-id="2106d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2106d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2106d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2106d-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2106d-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2106d-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="2106d-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="2106d-119">Function parameters</span></span>

<span data-ttu-id="2106d-120">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="2106d-120">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="2106d-121">参数</span><span class="sxs-lookup"><span data-stu-id="2106d-121">Parameter</span></span> | <span data-ttu-id="2106d-122">类型</span><span class="sxs-lookup"><span data-stu-id="2106d-122">Type</span></span>   | <span data-ttu-id="2106d-123">说明</span><span class="sxs-lookup"><span data-stu-id="2106d-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2106d-124">period</span><span class="sxs-lookup"><span data-stu-id="2106d-124">period</span></span>    | <span data-ttu-id="2106d-125">string</span><span class="sxs-lookup"><span data-stu-id="2106d-125">string</span></span> | <span data-ttu-id="2106d-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2106d-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2106d-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="2106d-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2106d-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2106d-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="2106d-129">必需。</span><span class="sxs-lookup"><span data-stu-id="2106d-129">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="2106d-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="2106d-130">Request headers</span></span>

| <span data-ttu-id="2106d-131">名称</span><span class="sxs-lookup"><span data-stu-id="2106d-131">Name</span></span>          | <span data-ttu-id="2106d-132">说明</span><span class="sxs-lookup"><span data-stu-id="2106d-132">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2106d-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="2106d-133">Authorization</span></span> | <span data-ttu-id="2106d-p103">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="2106d-p103">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2106d-136">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2106d-136">If-None-Match</span></span> | <span data-ttu-id="2106d-137">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2106d-137">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2106d-138">可选。</span><span class="sxs-lookup"><span data-stu-id="2106d-138">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2106d-139">响应</span><span class="sxs-lookup"><span data-stu-id="2106d-139">Response</span></span>

<span data-ttu-id="2106d-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2106d-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2106d-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2106d-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2106d-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="2106d-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2106d-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="2106d-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2106d-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2106d-144">Report Refresh Date</span></span>
- <span data-ttu-id="2106d-145">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="2106d-145">Mail For Mac</span></span>
- <span data-ttu-id="2106d-146">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="2106d-146">Outlook For Mac</span></span>
- <span data-ttu-id="2106d-147">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="2106d-147">Outlook For Windows</span></span>
- <span data-ttu-id="2106d-148">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="2106d-148">Outlook For Mobile</span></span>
- <span data-ttu-id="2106d-149">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="2106d-149">Other For Mobile</span></span>
- <span data-ttu-id="2106d-150">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="2106d-150">Outlook For Web</span></span>
- <span data-ttu-id="2106d-151">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="2106d-151">POP3 App</span></span>
- <span data-ttu-id="2106d-152">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="2106d-152">IMAP4 App</span></span>
- <span data-ttu-id="2106d-153">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="2106d-153">SMTP App</span></span>
- <span data-ttu-id="2106d-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="2106d-154">Report Date</span></span>
- <span data-ttu-id="2106d-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="2106d-155">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2106d-156">示例</span><span class="sxs-lookup"><span data-stu-id="2106d-156">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2106d-157">请求</span><span class="sxs-lookup"><span data-stu-id="2106d-157">Request</span></span>

<span data-ttu-id="2106d-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2106d-158">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getemailappusageusercounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getEmailAppUsageUserCounts(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2106d-159">C#</span><span class="sxs-lookup"><span data-stu-id="2106d-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2106d-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="2106d-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2106d-161">目标-C</span><span class="sxs-lookup"><span data-stu-id="2106d-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2106d-162">响应</span><span class="sxs-lookup"><span data-stu-id="2106d-162">Response</span></span>

<span data-ttu-id="2106d-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2106d-163">The following is an example of the response.</span></span>

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

<span data-ttu-id="2106d-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2106d-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
