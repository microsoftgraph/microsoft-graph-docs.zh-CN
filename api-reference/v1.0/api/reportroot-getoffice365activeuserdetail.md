---
title: 'reportRoot: getOffice365ActiveUserDetail'
description: 获取 Office 365 活跃用户的详细信息。
localization_priority: Priority
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 77bcab1728cede1721f28b38aaa5fec075816684
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729705"
---
# <a name="reportroot-getoffice365activeuserdetail"></a><span data-ttu-id="6f75a-103">reportRoot：getOffice365ActiveUserDetail</span><span class="sxs-lookup"><span data-stu-id="6f75a-103">reportRoot: getOffice365ActiveUserDetail</span></span>

<span data-ttu-id="6f75a-104">获取 Office 365 活跃用户的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6f75a-104">Get details about Office 365 active users.</span></span>

> <span data-ttu-id="6f75a-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="6f75a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="6f75a-106">权限</span><span class="sxs-lookup"><span data-stu-id="6f75a-106">Permissions</span></span>

<span data-ttu-id="6f75a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f75a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f75a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f75a-109">Permission type</span></span>                        | <span data-ttu-id="6f75a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f75a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6f75a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f75a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f75a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f75a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6f75a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f75a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f75a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f75a-114">Not supported.</span></span>                           |
| <span data-ttu-id="6f75a-115">应用</span><span class="sxs-lookup"><span data-stu-id="6f75a-115">Application</span></span>                            | <span data-ttu-id="6f75a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f75a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="6f75a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f75a-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOffice365ActiveUserDetail(period='{period_value}')
GET /reports/getOffice365ActiveUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="6f75a-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="6f75a-118">Function parameters</span></span>

<span data-ttu-id="6f75a-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="6f75a-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="6f75a-120">参数</span><span class="sxs-lookup"><span data-stu-id="6f75a-120">Parameter</span></span> | <span data-ttu-id="6f75a-121">类型</span><span class="sxs-lookup"><span data-stu-id="6f75a-121">Type</span></span>   | <span data-ttu-id="6f75a-122">说明</span><span class="sxs-lookup"><span data-stu-id="6f75a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6f75a-123">period</span><span class="sxs-lookup"><span data-stu-id="6f75a-123">period</span></span>    | <span data-ttu-id="6f75a-124">string</span><span class="sxs-lookup"><span data-stu-id="6f75a-124">string</span></span> | <span data-ttu-id="6f75a-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6f75a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6f75a-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6f75a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6f75a-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6f75a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6f75a-128">date</span><span class="sxs-lookup"><span data-stu-id="6f75a-128">date</span></span>      | <span data-ttu-id="6f75a-129">Date</span><span class="sxs-lookup"><span data-stu-id="6f75a-129">Date</span></span>   | <span data-ttu-id="6f75a-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="6f75a-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6f75a-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="6f75a-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6f75a-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="6f75a-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6f75a-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="6f75a-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f75a-134">请求头</span><span class="sxs-lookup"><span data-stu-id="6f75a-134">Request headers</span></span>

| <span data-ttu-id="6f75a-135">名称</span><span class="sxs-lookup"><span data-stu-id="6f75a-135">Name</span></span>          | <span data-ttu-id="6f75a-136">说明</span><span class="sxs-lookup"><span data-stu-id="6f75a-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="6f75a-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f75a-137">Authorization</span></span> | <span data-ttu-id="6f75a-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f75a-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="6f75a-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="6f75a-140">If-None-Match</span></span> | <span data-ttu-id="6f75a-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6f75a-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="6f75a-142">可选。</span><span class="sxs-lookup"><span data-stu-id="6f75a-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="6f75a-143">响应</span><span class="sxs-lookup"><span data-stu-id="6f75a-143">Response</span></span>

<span data-ttu-id="6f75a-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6f75a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6f75a-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6f75a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6f75a-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6f75a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6f75a-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6f75a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6f75a-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-148">Report Refresh Date</span></span>
- <span data-ttu-id="6f75a-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="6f75a-149">User Principal Name</span></span>
- <span data-ttu-id="6f75a-150">显示名称</span><span class="sxs-lookup"><span data-stu-id="6f75a-150">Display Name</span></span>
- <span data-ttu-id="6f75a-151">已删除</span><span class="sxs-lookup"><span data-stu-id="6f75a-151">Is Deleted</span></span>
- <span data-ttu-id="6f75a-152">删除日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-152">Deleted Date</span></span>
- <span data-ttu-id="6f75a-153">拥有 Exchange 许可证</span><span class="sxs-lookup"><span data-stu-id="6f75a-153">Has Exchange License</span></span>
- <span data-ttu-id="6f75a-154">拥有 OneDrive 许可证</span><span class="sxs-lookup"><span data-stu-id="6f75a-154">Has OneDrive License</span></span>
- <span data-ttu-id="6f75a-155">拥有 SharePoint 许可证</span><span class="sxs-lookup"><span data-stu-id="6f75a-155">Has SharePoint License</span></span>
- <span data-ttu-id="6f75a-156">拥有 Skype for Business 许可证</span><span class="sxs-lookup"><span data-stu-id="6f75a-156">Has Skype For Business License</span></span>
- <span data-ttu-id="6f75a-157">拥有 Yammer 许可证</span><span class="sxs-lookup"><span data-stu-id="6f75a-157">Has Yammer License</span></span>
- <span data-ttu-id="6f75a-158">拥有 Teams 许可证</span><span class="sxs-lookup"><span data-stu-id="6f75a-158">Has Teams License</span></span>
- <span data-ttu-id="6f75a-159">Exchange 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-159">Exchange Last Activity Date</span></span>
- <span data-ttu-id="6f75a-160">OneDrive 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-160">OneDrive Last Activity Date</span></span>
- <span data-ttu-id="6f75a-161">SharePoint 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-161">SharePoint Last Activity Date</span></span>
- <span data-ttu-id="6f75a-162">Skype for Business 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-162">Skype For Business Last Activity Date</span></span>
- <span data-ttu-id="6f75a-163">Yammer 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-163">Yammer Last Activity Date</span></span>
- <span data-ttu-id="6f75a-164">Teams 上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-164">Teams Last Activity Date</span></span>
- <span data-ttu-id="6f75a-165">Exchange 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-165">Exchange License Assign Date</span></span>
- <span data-ttu-id="6f75a-166">OneDrive 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-166">OneDrive License Assign Date</span></span>
- <span data-ttu-id="6f75a-167">SharePoint 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-167">SharePoint License Assign Date</span></span>
- <span data-ttu-id="6f75a-168">Skype for Business 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-168">Skype For Business License Assign Date</span></span>
- <span data-ttu-id="6f75a-169">Yammer 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-169">Yammer License Assign Date</span></span>
- <span data-ttu-id="6f75a-170">Teams 许可证分配日期</span><span class="sxs-lookup"><span data-stu-id="6f75a-170">Teams License Assign Date</span></span>
- <span data-ttu-id="6f75a-171">分配的产品</span><span class="sxs-lookup"><span data-stu-id="6f75a-171">Assigned Products</span></span>

## <a name="example"></a><span data-ttu-id="6f75a-172">示例</span><span class="sxs-lookup"><span data-stu-id="6f75a-172">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6f75a-173">请求</span><span class="sxs-lookup"><span data-stu-id="6f75a-173">Request</span></span>

<span data-ttu-id="6f75a-174">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6f75a-174">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6f75a-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f75a-175">--Http</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getoffice365activeuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActiveUserDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6f75a-176">C#</span><span class="sxs-lookup"><span data-stu-id="6f75a-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f75a-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f75a-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6f75a-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f75a-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6f75a-179">Java</span><span class="sxs-lookup"><span data-stu-id="6f75a-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getoffice365activeuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f75a-180">响应</span><span class="sxs-lookup"><span data-stu-id="6f75a-180">Response</span></span>

<span data-ttu-id="6f75a-181">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6f75a-181">The following is an example of the response.</span></span>

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

<span data-ttu-id="6f75a-182">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6f75a-182">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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
  ]
}-->
