---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: 获取组执行的 Office 365 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a165087479abdab0445a362524b31c3c531eb631
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268675"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="48dc9-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="48dc9-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="48dc9-104">获取组执行的 Office 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="48dc9-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="48dc9-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="48dc9-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="48dc9-106">权限</span><span class="sxs-lookup"><span data-stu-id="48dc9-106">Permissions</span></span>

<span data-ttu-id="48dc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="48dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48dc9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="48dc9-109">Permission type</span></span>                        | <span data-ttu-id="48dc9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="48dc9-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="48dc9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48dc9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48dc9-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="48dc9-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="48dc9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48dc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48dc9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="48dc9-114">Not supported.</span></span>                           |
| <span data-ttu-id="48dc9-115">应用</span><span class="sxs-lookup"><span data-stu-id="48dc9-115">Application</span></span>                            | <span data-ttu-id="48dc9-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="48dc9-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="48dc9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48dc9-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="48dc9-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="48dc9-118">Function parameters</span></span>

<span data-ttu-id="48dc9-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="48dc9-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="48dc9-120">参数</span><span class="sxs-lookup"><span data-stu-id="48dc9-120">Parameter</span></span> | <span data-ttu-id="48dc9-121">类型</span><span class="sxs-lookup"><span data-stu-id="48dc9-121">Type</span></span>   | <span data-ttu-id="48dc9-122">说明</span><span class="sxs-lookup"><span data-stu-id="48dc9-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="48dc9-123">period</span><span class="sxs-lookup"><span data-stu-id="48dc9-123">period</span></span>    | <span data-ttu-id="48dc9-124">string</span><span class="sxs-lookup"><span data-stu-id="48dc9-124">string</span></span> | <span data-ttu-id="48dc9-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="48dc9-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="48dc9-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="48dc9-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="48dc9-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="48dc9-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="48dc9-128">date</span><span class="sxs-lookup"><span data-stu-id="48dc9-128">date</span></span>      | <span data-ttu-id="48dc9-129">Date</span><span class="sxs-lookup"><span data-stu-id="48dc9-129">Date</span></span>   | <span data-ttu-id="48dc9-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="48dc9-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="48dc9-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="48dc9-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="48dc9-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="48dc9-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="48dc9-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="48dc9-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="48dc9-134">请求头</span><span class="sxs-lookup"><span data-stu-id="48dc9-134">Request headers</span></span>

| <span data-ttu-id="48dc9-135">名称</span><span class="sxs-lookup"><span data-stu-id="48dc9-135">Name</span></span>          | <span data-ttu-id="48dc9-136">说明</span><span class="sxs-lookup"><span data-stu-id="48dc9-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="48dc9-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="48dc9-137">Authorization</span></span> | <span data-ttu-id="48dc9-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="48dc9-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="48dc9-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="48dc9-140">If-None-Match</span></span> | <span data-ttu-id="48dc9-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="48dc9-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="48dc9-142">可选。</span><span class="sxs-lookup"><span data-stu-id="48dc9-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="48dc9-143">响应</span><span class="sxs-lookup"><span data-stu-id="48dc9-143">Response</span></span>

<span data-ttu-id="48dc9-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="48dc9-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="48dc9-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="48dc9-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="48dc9-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="48dc9-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="48dc9-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="48dc9-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="48dc9-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="48dc9-148">Report Refresh Date</span></span>
- <span data-ttu-id="48dc9-149">组显示名称</span><span class="sxs-lookup"><span data-stu-id="48dc9-149">Group Display Name</span></span>
- <span data-ttu-id="48dc9-150">已删除</span><span class="sxs-lookup"><span data-stu-id="48dc9-150">Is Deleted</span></span>
- <span data-ttu-id="48dc9-151">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="48dc9-151">Owner Principal Name</span></span>
- <span data-ttu-id="48dc9-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="48dc9-152">Last Activity Date</span></span>
- <span data-ttu-id="48dc9-153">组类型</span><span class="sxs-lookup"><span data-stu-id="48dc9-153">Group Type</span></span>
- <span data-ttu-id="48dc9-154">成员数</span><span class="sxs-lookup"><span data-stu-id="48dc9-154">Member Count</span></span>
- <span data-ttu-id="48dc9-155">外部成员数</span><span class="sxs-lookup"><span data-stu-id="48dc9-155">External Member Count</span></span>
- <span data-ttu-id="48dc9-156">已接收 Exchange 电子邮件数</span><span class="sxs-lookup"><span data-stu-id="48dc9-156">Exchange Received Email Count</span></span>
- <span data-ttu-id="48dc9-157">SharePoint 活跃文件数</span><span class="sxs-lookup"><span data-stu-id="48dc9-157">SharePoint Active File Count</span></span>
- <span data-ttu-id="48dc9-158">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="48dc9-158">Yammer Posted Message Count</span></span>
- <span data-ttu-id="48dc9-159">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="48dc9-159">Yammer Read Message Count</span></span>
- <span data-ttu-id="48dc9-160">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="48dc9-160">Yammer Liked Message Count</span></span>
- <span data-ttu-id="48dc9-161">Exchange 邮箱总项数</span><span class="sxs-lookup"><span data-stu-id="48dc9-161">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="48dc9-162">已使用的 Exchange 邮箱存储（字节）</span><span class="sxs-lookup"><span data-stu-id="48dc9-162">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="48dc9-163">SharePoint 文件总数</span><span class="sxs-lookup"><span data-stu-id="48dc9-163">SharePoint Total File Count</span></span>
- <span data-ttu-id="48dc9-164">已使用的 SharePoint 网站存储（字节）</span><span class="sxs-lookup"><span data-stu-id="48dc9-164">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="48dc9-165">报表周期</span><span class="sxs-lookup"><span data-stu-id="48dc9-165">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="48dc9-166">示例</span><span class="sxs-lookup"><span data-stu-id="48dc9-166">Example</span></span>

#### <a name="request"></a><span data-ttu-id="48dc9-167">请求</span><span class="sxs-lookup"><span data-stu-id="48dc9-167">Request</span></span>

<span data-ttu-id="48dc9-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="48dc9-168">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="48dc9-169">响应</span><span class="sxs-lookup"><span data-stu-id="48dc9-169">Response</span></span>

<span data-ttu-id="48dc9-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="48dc9-170">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="48dc9-171">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="48dc9-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="48dc9-172">C#</span><span class="sxs-lookup"><span data-stu-id="48dc9-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivityuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48dc9-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="48dc9-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivityuserdetail-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="48dc9-174">目标-C</span><span class="sxs-lookup"><span data-stu-id="48dc9-174">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365groupsactivityuserdetail-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="48dc9-175">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="48dc9-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Report Period
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365groupsactivitydetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
