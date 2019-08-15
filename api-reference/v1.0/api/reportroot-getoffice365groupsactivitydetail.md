---
title: 'reportRoot: getOffice365GroupsActivityDetail'
description: 获取组执行的 Office 365 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 5be09bba7a7867d0f994adecbed4e7690e20d61b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422296"
---
# <a name="reportroot-getoffice365groupsactivitydetail"></a><span data-ttu-id="89608-103">reportRoot: getOffice365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="89608-103">reportRoot: getOffice365GroupsActivityDetail</span></span>

<span data-ttu-id="89608-104">获取组执行的 Office 365 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="89608-104">Get details about Office 365 Groups activity by group.</span></span>

> <span data-ttu-id="89608-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="89608-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="89608-106">权限</span><span class="sxs-lookup"><span data-stu-id="89608-106">Permissions</span></span>

<span data-ttu-id="89608-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89608-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89608-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="89608-109">Permission type</span></span>                        | <span data-ttu-id="89608-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89608-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="89608-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89608-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="89608-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="89608-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="89608-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89608-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89608-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="89608-114">Not supported.</span></span>                           |
| <span data-ttu-id="89608-115">应用</span><span class="sxs-lookup"><span data-stu-id="89608-115">Application</span></span>                            | <span data-ttu-id="89608-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="89608-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="89608-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89608-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365GroupsActivityDetail(period='{period_value}')
GET /reports/getOffice365GroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="89608-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="89608-118">Function parameters</span></span>

<span data-ttu-id="89608-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="89608-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="89608-120">参数</span><span class="sxs-lookup"><span data-stu-id="89608-120">Parameter</span></span> | <span data-ttu-id="89608-121">类型</span><span class="sxs-lookup"><span data-stu-id="89608-121">Type</span></span>   | <span data-ttu-id="89608-122">说明</span><span class="sxs-lookup"><span data-stu-id="89608-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="89608-123">period</span><span class="sxs-lookup"><span data-stu-id="89608-123">period</span></span>    | <span data-ttu-id="89608-124">string</span><span class="sxs-lookup"><span data-stu-id="89608-124">string</span></span> | <span data-ttu-id="89608-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="89608-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="89608-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="89608-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="89608-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="89608-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="89608-128">date</span><span class="sxs-lookup"><span data-stu-id="89608-128">date</span></span>      | <span data-ttu-id="89608-129">Date</span><span class="sxs-lookup"><span data-stu-id="89608-129">Date</span></span>   | <span data-ttu-id="89608-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="89608-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="89608-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="89608-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="89608-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="89608-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="89608-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="89608-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89608-134">请求头</span><span class="sxs-lookup"><span data-stu-id="89608-134">Request headers</span></span>

| <span data-ttu-id="89608-135">名称</span><span class="sxs-lookup"><span data-stu-id="89608-135">Name</span></span>          | <span data-ttu-id="89608-136">说明</span><span class="sxs-lookup"><span data-stu-id="89608-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="89608-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="89608-137">Authorization</span></span> | <span data-ttu-id="89608-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="89608-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="89608-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="89608-140">If-None-Match</span></span> | <span data-ttu-id="89608-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="89608-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="89608-142">可选。</span><span class="sxs-lookup"><span data-stu-id="89608-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="89608-143">响应</span><span class="sxs-lookup"><span data-stu-id="89608-143">Response</span></span>

<span data-ttu-id="89608-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="89608-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="89608-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="89608-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="89608-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="89608-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="89608-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="89608-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="89608-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="89608-148">Report Refresh Date</span></span>
- <span data-ttu-id="89608-149">组显示名称</span><span class="sxs-lookup"><span data-stu-id="89608-149">Group Display Name</span></span>
- <span data-ttu-id="89608-150">已删除</span><span class="sxs-lookup"><span data-stu-id="89608-150">Is Deleted</span></span>
- <span data-ttu-id="89608-151">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="89608-151">Owner Principal Name</span></span>
- <span data-ttu-id="89608-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="89608-152">Last Activity Date</span></span>
- <span data-ttu-id="89608-153">组类型</span><span class="sxs-lookup"><span data-stu-id="89608-153">Group Type</span></span>
- <span data-ttu-id="89608-154">成员数</span><span class="sxs-lookup"><span data-stu-id="89608-154">Member Count</span></span>
- <span data-ttu-id="89608-155">外部成员数</span><span class="sxs-lookup"><span data-stu-id="89608-155">External Member Count</span></span>
- <span data-ttu-id="89608-156">已接收 Exchange 电子邮件数</span><span class="sxs-lookup"><span data-stu-id="89608-156">Exchange Received Email Count</span></span>
- <span data-ttu-id="89608-157">SharePoint 活跃文件数</span><span class="sxs-lookup"><span data-stu-id="89608-157">SharePoint Active File Count</span></span>
- <span data-ttu-id="89608-158">已发布 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="89608-158">Yammer Posted Message Count</span></span>
- <span data-ttu-id="89608-159">已阅读 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="89608-159">Yammer Read Message Count</span></span>
- <span data-ttu-id="89608-160">已赞 Yammer 消息数</span><span class="sxs-lookup"><span data-stu-id="89608-160">Yammer Liked Message Count</span></span>
- <span data-ttu-id="89608-161">Exchange 邮箱总项数</span><span class="sxs-lookup"><span data-stu-id="89608-161">Exchange Mailbox Total Item Count</span></span>
- <span data-ttu-id="89608-162">已使用的 Exchange 邮箱存储（字节）</span><span class="sxs-lookup"><span data-stu-id="89608-162">Exchange Mailbox Storage Used (Byte)</span></span>
- <span data-ttu-id="89608-163">SharePoint 文件总数</span><span class="sxs-lookup"><span data-stu-id="89608-163">SharePoint Total File Count</span></span>
- <span data-ttu-id="89608-164">已使用的 SharePoint 网站存储（字节）</span><span class="sxs-lookup"><span data-stu-id="89608-164">SharePoint Site Storage Used (Byte)</span></span>
- <span data-ttu-id="89608-165">组 Id</span><span class="sxs-lookup"><span data-stu-id="89608-165">Group Id</span></span>
- <span data-ttu-id="89608-166">报表周期</span><span class="sxs-lookup"><span data-stu-id="89608-166">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="89608-167">示例</span><span class="sxs-lookup"><span data-stu-id="89608-167">Example</span></span>

#### <a name="request"></a><span data-ttu-id="89608-168">请求</span><span class="sxs-lookup"><span data-stu-id="89608-168">Request</span></span>

<span data-ttu-id="89608-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89608-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="89608-170">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="89608-170">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365groupsactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365GroupsActivityDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89608-171">C#</span><span class="sxs-lookup"><span data-stu-id="89608-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89608-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89608-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89608-173">目标-C</span><span class="sxs-lookup"><span data-stu-id="89608-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="89608-174">Java</span><span class="sxs-lookup"><span data-stu-id="89608-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365groupsactivityuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="89608-175">响应</span><span class="sxs-lookup"><span data-stu-id="89608-175">Response</span></span>

<span data-ttu-id="89608-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="89608-176">The following is an example of the response.</span></span>

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

<span data-ttu-id="89608-177">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="89608-177">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Member Count,Guest Count,Exchange Received Email Count,SharePoint Active File Count,Yammer Posted Message Count,Yammer Read Message Count,Yammer Liked Message Count,Exchange Mailbox Total Item Count,Exchange Mailbox Storage Used (Byte),SharePoint Total File Count,SharePoint Site Storage Used (Byte),Group Id,Report Period
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
