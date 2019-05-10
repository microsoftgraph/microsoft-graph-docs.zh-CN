---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: 获取 Office 365 活跃用户的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 134ec4804a17bc70d16246474bc4de6b7514eb93
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33606604"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="6c2ec-103">reportRoot：getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="6c2ec-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="6c2ec-104">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="6c2ec-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="6c2ec-106">权限</span><span class="sxs-lookup"><span data-stu-id="6c2ec-106">Permissions</span></span>

<span data-ttu-id="6c2ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c2ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c2ec-109">Permission type</span></span>                        | <span data-ttu-id="6c2ec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c2ec-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6c2ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c2ec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c2ec-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c2ec-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6c2ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c2ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c2ec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-114">Not supported.</span></span>                           |
| <span data-ttu-id="6c2ec-115">应用</span><span class="sxs-lookup"><span data-stu-id="6c2ec-115">Application</span></span>                            | <span data-ttu-id="6c2ec-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c2ec-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6c2ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c2ec-117">HTTP request</span></span>

<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="6c2ec-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="6c2ec-118">Function parameters</span></span>

<span data-ttu-id="6c2ec-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="6c2ec-120">参数</span><span class="sxs-lookup"><span data-stu-id="6c2ec-120">Parameter</span></span> | <span data-ttu-id="6c2ec-121">类型</span><span class="sxs-lookup"><span data-stu-id="6c2ec-121">Type</span></span>   | <span data-ttu-id="6c2ec-122">说明</span><span class="sxs-lookup"><span data-stu-id="6c2ec-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6c2ec-123">period</span><span class="sxs-lookup"><span data-stu-id="6c2ec-123">period</span></span>    | <span data-ttu-id="6c2ec-124">string</span><span class="sxs-lookup"><span data-stu-id="6c2ec-124">string</span></span> | <span data-ttu-id="6c2ec-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6c2ec-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6c2ec-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6c2ec-128">date</span><span class="sxs-lookup"><span data-stu-id="6c2ec-128">date</span></span>      | <span data-ttu-id="6c2ec-129">Date</span><span class="sxs-lookup"><span data-stu-id="6c2ec-129">Date</span></span>   | <span data-ttu-id="6c2ec-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6c2ec-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6c2ec-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6c2ec-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c2ec-134">请求头</span><span class="sxs-lookup"><span data-stu-id="6c2ec-134">Request headers</span></span>

| <span data-ttu-id="6c2ec-135">名称</span><span class="sxs-lookup"><span data-stu-id="6c2ec-135">Name</span></span>          | <span data-ttu-id="6c2ec-136">说明</span><span class="sxs-lookup"><span data-stu-id="6c2ec-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6c2ec-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c2ec-137">Authorization</span></span> | <span data-ttu-id="6c2ec-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6c2ec-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6c2ec-140">If-None-Match</span></span> | <span data-ttu-id="6c2ec-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6c2ec-142">可选。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6c2ec-143">响应</span><span class="sxs-lookup"><span data-stu-id="6c2ec-143">Response</span></span>

<span data-ttu-id="6c2ec-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6c2ec-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6c2ec-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6c2ec-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6c2ec-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-148">Report Refresh Date</span></span>
- <span data-ttu-id="6c2ec-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="6c2ec-149">User Principal Name</span></span>
- <span data-ttu-id="6c2ec-150">显示名称</span><span class="sxs-lookup"><span data-stu-id="6c2ec-150">Display Name</span></span>
- <span data-ttu-id="6c2ec-151">已删除</span><span class="sxs-lookup"><span data-stu-id="6c2ec-151">Is Deleted</span></span>
- <span data-ttu-id="6c2ec-152">删除日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-152">Deleted Date</span></span>
- <span data-ttu-id="6c2ec-153">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="6c2ec-153">Has Exchange License</span></span>
- <span data-ttu-id="6c2ec-154">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="6c2ec-154">Has OneDrive License</span></span>
- <span data-ttu-id="6c2ec-155">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="6c2ec-155">Has SharePoint License</span></span>
- <span data-ttu-id="6c2ec-156">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="6c2ec-156">Has Skype For Business License</span></span>
- <span data-ttu-id="6c2ec-157">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="6c2ec-157">Has Yammer License</span></span>
- <span data-ttu-id="6c2ec-158">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="6c2ec-158">Has Teams License</span></span>
- <span data-ttu-id="6c2ec-159">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-159">Exchange Last Activity Date</span></span>
- <span data-ttu-id="6c2ec-160">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-160">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="6c2ec-161">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-161">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="6c2ec-162">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-162">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="6c2ec-163">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-163">Yammer Last Activity Date</span></span>
- <span data-ttu-id="6c2ec-164">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-164">Teams Last Activity Date</span></span>
- <span data-ttu-id="6c2ec-165">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-165">Exchange License Assign Date</span></span>
- <span data-ttu-id="6c2ec-166">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-166">OneDrive License Assign Date</span></span>
- <span data-ttu-id="6c2ec-167">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-167">SharePoint License Assign Date</span></span>
- <span data-ttu-id="6c2ec-168">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-168">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="6c2ec-169">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-169">Yammer License Assign Date</span></span>
- <span data-ttu-id="6c2ec-170">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6c2ec-170">Teams License Assign Date</span></span>
- <span data-ttu-id="6c2ec-171">分配的产品</span><span class="sxs-lookup"><span data-stu-id="6c2ec-171">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="6c2ec-172">示例</span><span class="sxs-lookup"><span data-stu-id="6c2ec-172">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6c2ec-173">请求</span><span class="sxs-lookup"><span data-stu-id="6c2ec-173">Request</span></span>

<span data-ttu-id="6c2ec-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-174">The following is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="6c2ec-175">响应</span><span class="sxs-lookup"><span data-stu-id="6c2ec-175">Response</span></span>

<span data-ttu-id="6c2ec-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-176">The following is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6c2ec-177">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6c2ec-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6c2ec-178">C#</span><span class="sxs-lookup"><span data-stu-id="6c2ec-178">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6c2ec-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="6c2ec-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getoffice365activeuserdetail-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="6c2ec-180">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6c2ec-180">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Has Exchange License,Has OneDrive License,Has SharePoint License,Has Skype For Business License,Has Yammer License,Has Teams License,Exchange Last Activity Date,OneDrive Last Activity Date,SharePoint Last Activity Date,Skype For Business Last Activity Date,Yammer Last Activity Date,Teams Last Activity Date,Exchange License Assign Date,OneDrive License Assign Date,SharePoint License Assign Date,Skype For Business License Assign Date,Yammer License Assign Date,Teams License Assign Date,Assigned Products
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
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/reportroot-getoffice365activeuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
