---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: 获取帐户的 OneDrive 使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0d08c2b86030f7ca0b4bdff83f99e5e5f6a6179e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728109"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="2ed35-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="2ed35-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

<span data-ttu-id="2ed35-104">获取帐户的 OneDrive 使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2ed35-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="2ed35-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="2ed35-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="2ed35-106">权限</span><span class="sxs-lookup"><span data-stu-id="2ed35-106">Permissions</span></span>

<span data-ttu-id="2ed35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ed35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ed35-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ed35-109">Permission type</span></span>                        | <span data-ttu-id="2ed35-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ed35-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="2ed35-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed35-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ed35-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ed35-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="2ed35-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed35-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ed35-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ed35-114">Not supported.</span></span>                           |
| <span data-ttu-id="2ed35-115">应用</span><span class="sxs-lookup"><span data-stu-id="2ed35-115">Application</span></span>                            | <span data-ttu-id="2ed35-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ed35-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2ed35-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ed35-117">HTTP request</span></span>


<!-- { "blockType": "samples" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="2ed35-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="2ed35-118">Function parameters</span></span>

<span data-ttu-id="2ed35-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="2ed35-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="2ed35-120">参数</span><span class="sxs-lookup"><span data-stu-id="2ed35-120">Parameter</span></span> | <span data-ttu-id="2ed35-121">类型</span><span class="sxs-lookup"><span data-stu-id="2ed35-121">Type</span></span>   | <span data-ttu-id="2ed35-122">说明</span><span class="sxs-lookup"><span data-stu-id="2ed35-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="2ed35-123">period</span><span class="sxs-lookup"><span data-stu-id="2ed35-123">period</span></span>    | <span data-ttu-id="2ed35-124">string</span><span class="sxs-lookup"><span data-stu-id="2ed35-124">string</span></span> | <span data-ttu-id="2ed35-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2ed35-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="2ed35-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="2ed35-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="2ed35-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="2ed35-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="2ed35-128">date</span><span class="sxs-lookup"><span data-stu-id="2ed35-128">date</span></span>      | <span data-ttu-id="2ed35-129">Date</span><span class="sxs-lookup"><span data-stu-id="2ed35-129">Date</span></span>   | <span data-ttu-id="2ed35-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="2ed35-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="2ed35-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="2ed35-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="2ed35-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="2ed35-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="2ed35-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="2ed35-133">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ed35-134">请求头</span><span class="sxs-lookup"><span data-stu-id="2ed35-134">Request headers</span></span>

| <span data-ttu-id="2ed35-135">名称</span><span class="sxs-lookup"><span data-stu-id="2ed35-135">Name</span></span>          | <span data-ttu-id="2ed35-136">说明</span><span class="sxs-lookup"><span data-stu-id="2ed35-136">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="2ed35-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ed35-137">Authorization</span></span> | <span data-ttu-id="2ed35-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ed35-p104">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="2ed35-140">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="2ed35-140">If-None-Match</span></span> | <span data-ttu-id="2ed35-141">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2ed35-141">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="2ed35-142">可选。</span><span class="sxs-lookup"><span data-stu-id="2ed35-142">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="2ed35-143">响应</span><span class="sxs-lookup"><span data-stu-id="2ed35-143">Response</span></span>

<span data-ttu-id="2ed35-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="2ed35-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="2ed35-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="2ed35-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="2ed35-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="2ed35-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="2ed35-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="2ed35-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="2ed35-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="2ed35-148">Report Refresh Date</span></span>
- <span data-ttu-id="2ed35-149">网站 URL</span><span class="sxs-lookup"><span data-stu-id="2ed35-149">Site URL</span></span>
- <span data-ttu-id="2ed35-150">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="2ed35-150">Owner Display Name</span></span>
- <span data-ttu-id="2ed35-151">已删除</span><span class="sxs-lookup"><span data-stu-id="2ed35-151">Is Deleted</span></span>
- <span data-ttu-id="2ed35-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="2ed35-152">Last Activity Date</span></span>
- <span data-ttu-id="2ed35-153">文件数</span><span class="sxs-lookup"><span data-stu-id="2ed35-153">File Count</span></span>
- <span data-ttu-id="2ed35-154">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="2ed35-154">Active File Count</span></span>
- <span data-ttu-id="2ed35-155">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="2ed35-155">Storage Used (Byte)</span></span>
- <span data-ttu-id="2ed35-156">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="2ed35-156">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="2ed35-157">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="2ed35-157">Owner Principal Name</span></span>
- <span data-ttu-id="2ed35-158">报表周期</span><span class="sxs-lookup"><span data-stu-id="2ed35-158">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="2ed35-159">示例</span><span class="sxs-lookup"><span data-stu-id="2ed35-159">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2ed35-160">请求</span><span class="sxs-lookup"><span data-stu-id="2ed35-160">Request</span></span>

<span data-ttu-id="2ed35-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2ed35-161">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2ed35-162">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2ed35-162">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "reportroot_getonedriveusageuserdetail"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/reports/getOneDriveUsageAccountDetail(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ed35-163">C#</span><span class="sxs-lookup"><span data-stu-id="2ed35-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageuserdetail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ed35-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ed35-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageuserdetail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ed35-165">目标-C</span><span class="sxs-lookup"><span data-stu-id="2ed35-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageuserdetail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2ed35-166">Java</span><span class="sxs-lookup"><span data-stu-id="2ed35-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveusageuserdetail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2ed35-167">响应</span><span class="sxs-lookup"><span data-stu-id="2ed35-167">Response</span></span>

<span data-ttu-id="2ed35-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2ed35-168">The following is an example of the response.</span></span>

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

<span data-ttu-id="2ed35-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="2ed35-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
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
