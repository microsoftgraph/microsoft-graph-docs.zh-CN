---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: 获取组执行的 Office 365 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a1fd2fd17e65d508c6548e6f5cdeb4dae7984a9b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893951"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="b3d70-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="b3d70-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="b3d70-104">获取组执行的 Office 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b3d70-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="b3d70-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="b3d70-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3d70-106">权限</span><span class="sxs-lookup"><span data-stu-id="b3d70-106">Permissions</span></span>

<span data-ttu-id="b3d70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3d70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3d70-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3d70-109">Permission type</span></span>                        | <span data-ttu-id="b3d70-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3d70-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b3d70-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3d70-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3d70-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3d70-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b3d70-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3d70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3d70-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3d70-114">Not supported.</span></span>                           |
| <span data-ttu-id="b3d70-115">应用</span><span class="sxs-lookup"><span data-stu-id="b3d70-115">Application</span></span>                            | <span data-ttu-id="b3d70-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3d70-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b3d70-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3d70-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b3d70-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b3d70-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="b3d70-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="b3d70-119">Function parameters</span></span>

<span data-ttu-id="b3d70-120">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b3d70-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="b3d70-121">参数</span><span class="sxs-lookup"><span data-stu-id="b3d70-121">Parameter</span></span> | <span data-ttu-id="b3d70-122">类型</span><span class="sxs-lookup"><span data-stu-id="b3d70-122">Type</span></span>   | <span data-ttu-id="b3d70-123">说明</span><span class="sxs-lookup"><span data-stu-id="b3d70-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b3d70-124">period</span><span class="sxs-lookup"><span data-stu-id="b3d70-124">period</span></span>    | <span data-ttu-id="b3d70-125">string</span><span class="sxs-lookup"><span data-stu-id="b3d70-125">string</span></span> | <span data-ttu-id="b3d70-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b3d70-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b3d70-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b3d70-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b3d70-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b3d70-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="b3d70-129">date</span><span class="sxs-lookup"><span data-stu-id="b3d70-129">date</span></span>      | <span data-ttu-id="b3d70-130">Date</span><span class="sxs-lookup"><span data-stu-id="b3d70-130">Date</span></span>   | <span data-ttu-id="b3d70-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="b3d70-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="b3d70-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="b3d70-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="b3d70-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="b3d70-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="b3d70-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="b3d70-134">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3d70-135">请求头</span><span class="sxs-lookup"><span data-stu-id="b3d70-135">Request headers</span></span>

| <span data-ttu-id="b3d70-136">名称</span><span class="sxs-lookup"><span data-stu-id="b3d70-136">Name</span></span>          | <span data-ttu-id="b3d70-137">说明</span><span class="sxs-lookup"><span data-stu-id="b3d70-137">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="b3d70-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3d70-138">Authorization</span></span> | <span data-ttu-id="b3d70-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3d70-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="b3d70-141">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b3d70-141">If-None-Match</span></span> | <span data-ttu-id="b3d70-142">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b3d70-142">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b3d70-143">可选。</span><span class="sxs-lookup"><span data-stu-id="b3d70-143">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b3d70-144">响应</span><span class="sxs-lookup"><span data-stu-id="b3d70-144">Response</span></span>

<span data-ttu-id="b3d70-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b3d70-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b3d70-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b3d70-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b3d70-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b3d70-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b3d70-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b3d70-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b3d70-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b3d70-149">Report Refresh Date</span></span>
- <span data-ttu-id="b3d70-150">组显示名称</span><span class="sxs-lookup"><span data-stu-id="b3d70-150">Group Display Name</span></span>
- <span data-ttu-id="b3d70-151">已删除</span><span class="sxs-lookup"><span data-stu-id="b3d70-151">Is Deleted</span></span>
- <span data-ttu-id="b3d70-152">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="b3d70-152">Owner Principal Name</span></span>
- <span data-ttu-id="b3d70-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="b3d70-153">Last Activity Date</span></span>
- <span data-ttu-id="b3d70-154">组类型</span><span class="sxs-lookup"><span data-stu-id="b3d70-154">Group Type</span></span>
- <span data-ttu-id="b3d70-155">成员数</span><span class="sxs-lookup"><span data-stu-id="b3d70-155">Member Count</span></span>
- <span data-ttu-id="b3d70-156">外部成员数</span><span class="sxs-lookup"><span data-stu-id="b3d70-156">External Member Count</span></span>
- <span data-ttu-id="b3d70-157">已接收 Exchange 电子邮件数</span><span class="sxs-lookup"><span data-stu-id="b3d70-157">Exchange Received Email Count</span></span>
- <span data-ttu-id="b3d70-158">SharePoint 活跃文件数</span><span class="sxs-lookup"><span data-stu-id="b3d70-158">SharePoint Active File Count</span></span>
- <span data-ttu-id="b3d70-159">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="b3d70-159">Yammer Posted Message Count</span></span>
- <span data-ttu-id="b3d70-160">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="b3d70-160">Yammer Read Message Count</span></span>
- <span data-ttu-id="b3d70-161">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="b3d70-161">Yammer Liked Message Count</span></span>
- <span data-ttu-id="b3d70-162">Exchange 邮箱总项数</span><span class="sxs-lookup"><span data-stu-id="b3d70-162">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="b3d70-163">已使用的 Exchange 邮箱存储（字节）</span><span class="sxs-lookup"><span data-stu-id="b3d70-163">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="b3d70-164">SharePoint 文件总数</span><span class="sxs-lookup"><span data-stu-id="b3d70-164">SharePoint Total File Count</span></span>
- <span data-ttu-id="b3d70-165">已使用的 SharePoint 网站存储（字节）</span><span class="sxs-lookup"><span data-stu-id="b3d70-165">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="b3d70-166">报表周期</span><span class="sxs-lookup"><span data-stu-id="b3d70-166">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="b3d70-167">示例</span><span class="sxs-lookup"><span data-stu-id="b3d70-167">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b3d70-168">请求</span><span class="sxs-lookup"><span data-stu-id="b3d70-168">Request</span></span>

<span data-ttu-id="b3d70-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b3d70-169">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3d70-170">C#</span><span class="sxs-lookup"><span data-stu-id="b3d70-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3d70-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="b3d70-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3d70-172">目标-C</span><span class="sxs-lookup"><span data-stu-id="b3d70-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b3d70-173">Java</span><span class="sxs-lookup"><span data-stu-id="b3d70-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b3d70-174">响应</span><span class="sxs-lookup"><span data-stu-id="b3d70-174">Response</span></span>

<span data-ttu-id="b3d70-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b3d70-175">The following is an example of the response.</span></span>

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

<span data-ttu-id="b3d70-176">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b3d70-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
