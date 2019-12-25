---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: 获取 SharePoint 网站使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b396cbfe22bf4ce2294d6507860b2d06f83a3676
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865347"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="5e6df-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="5e6df-103">reportRoot: getSharePointSiteUsageDetail</span></span>

<span data-ttu-id="5e6df-104">获取 SharePoint 网站使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5e6df-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="5e6df-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="5e6df-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e6df-106">权限</span><span class="sxs-lookup"><span data-stu-id="5e6df-106">Permissions</span></span>

<span data-ttu-id="5e6df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e6df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e6df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e6df-109">Permission type</span></span>                        | <span data-ttu-id="5e6df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e6df-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5e6df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e6df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e6df-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e6df-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5e6df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e6df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e6df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e6df-114">Not supported.</span></span>                           |
| <span data-ttu-id="5e6df-115">应用</span><span class="sxs-lookup"><span data-stu-id="5e6df-115">Application</span></span>                            | <span data-ttu-id="5e6df-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e6df-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="5e6df-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="5e6df-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="5e6df-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="5e6df-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="5e6df-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e6df-119">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="5e6df-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="5e6df-120">Function parameters</span></span>

<span data-ttu-id="5e6df-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="5e6df-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="5e6df-122">参数</span><span class="sxs-lookup"><span data-stu-id="5e6df-122">Parameter</span></span> | <span data-ttu-id="5e6df-123">类型</span><span class="sxs-lookup"><span data-stu-id="5e6df-123">Type</span></span>   | <span data-ttu-id="5e6df-124">说明</span><span class="sxs-lookup"><span data-stu-id="5e6df-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5e6df-125">period</span><span class="sxs-lookup"><span data-stu-id="5e6df-125">period</span></span>    | <span data-ttu-id="5e6df-126">string</span><span class="sxs-lookup"><span data-stu-id="5e6df-126">string</span></span> | <span data-ttu-id="5e6df-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5e6df-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5e6df-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="5e6df-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5e6df-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5e6df-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="5e6df-130">date</span><span class="sxs-lookup"><span data-stu-id="5e6df-130">date</span></span>      | <span data-ttu-id="5e6df-131">Date</span><span class="sxs-lookup"><span data-stu-id="5e6df-131">Date</span></span>   | <span data-ttu-id="5e6df-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="5e6df-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="5e6df-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="5e6df-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="5e6df-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="5e6df-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="5e6df-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="5e6df-135">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e6df-136">请求头</span><span class="sxs-lookup"><span data-stu-id="5e6df-136">Request headers</span></span>

| <span data-ttu-id="5e6df-137">名称</span><span class="sxs-lookup"><span data-stu-id="5e6df-137">Name</span></span>          | <span data-ttu-id="5e6df-138">说明</span><span class="sxs-lookup"><span data-stu-id="5e6df-138">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="5e6df-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e6df-139">Authorization</span></span> | <span data-ttu-id="5e6df-p105">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e6df-p105">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="5e6df-142">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="5e6df-142">If-None-Match</span></span> | <span data-ttu-id="5e6df-143">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5e6df-143">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="5e6df-144">可选。</span><span class="sxs-lookup"><span data-stu-id="5e6df-144">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="5e6df-145">响应</span><span class="sxs-lookup"><span data-stu-id="5e6df-145">Response</span></span>

<span data-ttu-id="5e6df-146">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5e6df-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5e6df-147">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="5e6df-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5e6df-148">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="5e6df-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5e6df-149">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="5e6df-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5e6df-150">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="5e6df-150">Report Refresh Date</span></span>
- <span data-ttu-id="5e6df-151">网站 Id</span><span class="sxs-lookup"><span data-stu-id="5e6df-151">Site Id</span></span>
- <span data-ttu-id="5e6df-152">网站 URL</span><span class="sxs-lookup"><span data-stu-id="5e6df-152">Site URL</span></span>
- <span data-ttu-id="5e6df-153">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="5e6df-153">Owner Display Name</span></span>
- <span data-ttu-id="5e6df-154">已删除</span><span class="sxs-lookup"><span data-stu-id="5e6df-154">Is Deleted</span></span>
- <span data-ttu-id="5e6df-155">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="5e6df-155">Last Activity Date</span></span>
- <span data-ttu-id="5e6df-156">文件数</span><span class="sxs-lookup"><span data-stu-id="5e6df-156">File Count</span></span>
- <span data-ttu-id="5e6df-157">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="5e6df-157">Active File Count</span></span>
- <span data-ttu-id="5e6df-158">页面浏览量</span><span class="sxs-lookup"><span data-stu-id="5e6df-158">Page View Count</span></span>
- <span data-ttu-id="5e6df-159">访问过的页面数</span><span class="sxs-lookup"><span data-stu-id="5e6df-159">Visited Page Count</span></span>
- <span data-ttu-id="5e6df-160">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="5e6df-160">Storage Used (Byte)</span></span>
- <span data-ttu-id="5e6df-161">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="5e6df-161">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="5e6df-162">根网站模板</span><span class="sxs-lookup"><span data-stu-id="5e6df-162">Root Web Template</span></span>
- <span data-ttu-id="5e6df-163">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="5e6df-163">Owner Principal Name</span></span>
- <span data-ttu-id="5e6df-164">报表周期</span><span class="sxs-lookup"><span data-stu-id="5e6df-164">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="5e6df-165">示例</span><span class="sxs-lookup"><span data-stu-id="5e6df-165">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5e6df-166">请求</span><span class="sxs-lookup"><span data-stu-id="5e6df-166">Request</span></span>

<span data-ttu-id="5e6df-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e6df-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5e6df-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e6df-168">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getsharepointsiteusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getSharePointSiteUsageDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5e6df-169">C#</span><span class="sxs-lookup"><span data-stu-id="5e6df-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e6df-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e6df-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e6df-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e6df-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5e6df-172">Java</span><span class="sxs-lookup"><span data-stu-id="5e6df-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5e6df-173">响应</span><span class="sxs-lookup"><span data-stu-id="5e6df-173">Response</span></span>

<span data-ttu-id="5e6df-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5e6df-174">The following is an example of the response.</span></span>

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

<span data-ttu-id="5e6df-175">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="5e6df-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
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
